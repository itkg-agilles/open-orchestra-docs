Install OpenOrchestra with vagrant for contributors
===================================================

Open Orchestra is composed of three projects: 

- *open-orchestra* which is the CMS Back Office;
- *open-orchestra-front-demo* which is the Front Office part that will display the sites and pages
  created in the CMS Back Office;
- *open-orchestra-media-demo* which will display the images loaded in the CMS Back Office.

For contributors, we provide a Vagrant-powered environment with provisioning so you get minimal
setup actions to do.

Install Vagrant
---------------
The project is running on a Vagrant virtual environment built on VirtualBox to be production ready.

.. code-block:: bash

    $ aptitude install virtualbox
    $ wget https://dl.bintray.com/mitchellh/vagrant/vagrant_1.6.3_x86_64.deb
    $ dpkg -i vagrant_1.6.3_x86_64.deb

Install ansible
---------------

All the project server configuration is going to be handled by ansible.

Our configuration was made for the 1.9.4 version of ansible.

For more information about ansible installation, you can see `Ansible installation documentation`_.


Install nfs server
------------------

To improve the vagrant box performance, we share the folders with the ``nfs`` protocol. You need to
install a nfs server instance on your computer.

.. code-block:: bash

    $ aptitude install nfs-kernel-server

Download Composer
-----------------

Composer is the package manager used by modern PHP applications.

To install composer with curl:

.. code-block:: bash

    $ curl -sS https://getcomposer.org/installer | php

If you don't have curl installed, you can also download it with php:

.. code-block:: bash

    $ php -r "readfile('https://getcomposer.org/installer');" | php

see `Download Composer`_

Install OpenOrchestra
---------------------

To contribute on the project you have to install two versions: the master version and the last 
stable one. The master branch is the branch which should be used to add new features to the project.
Here is the directory tree with your two projects that we recommand:

.. code-block:: none

    |_ install-directory
          |_ open-orchestra-master
                |_ open-orchestra
                |_ open-orchestra-front-demo
                |_ open-orchestra-media-demo
                |_ open-orchestra-provision
          |_ open-orchestra-stable
                |_ open-orchestra
                |_ open-orchestra-front-demo
                |_ open-orchestra-media-demo
                |_ open-orchestra-provision

- To install the master open-orchestra parts using ``composer``:

  In your ``open-orchestra-master`` directory:
  
  .. code-block:: bash

    $ [path-to-composer]/composer.phar create-project open-orchestra/open-orchestra ./open-orchestra -s dev --ignore-platform-reqs --no-scripts --keep-vcs dev-master
    $ [path-to-composer]/composer.phar create-project open-orchestra/open-orchestra-front-demo ./open-orchestra-front-demo -s dev --ignore-platform-reqs --no-scripts --keep-vcs dev-master
    $ [path-to-composer]/composer.phar create-project open-orchestra/open-orchestra-media-demo ./open-orchestra-media-demo -s dev --ignore-platform-reqs --no-scripts --keep-vcs dev-master

  Clone the provisioning repository:

  .. code-block:: bash

    $ git clone git@github.com:open-orchestra/open-orchestra-provision.git

- To install the stable open-orchestra parts using ``composer``:

  In your ``open-orchestra-stable`` directory:
  
  .. code-block:: bash

    $ [path-to-composer]/composer.phar create-project open-orchestra/open-orchestra ./open-orchestra -s stable --ignore-platform-reqs --no-scripts --keep-vcs
    $ [path-to-composer]/composer.phar create-project open-orchestra/open-orchestra-front-demo ./open-orchestra-front-demo -s stable --ignore-platform-reqs --no-scripts --keep-vcs
    $ [path-to-composer]/composer.phar create-project open-orchestra/open-orchestra-media-demo ./open-orchestra-media-demo -s stable --ignore-platform-reqs --no-scripts --keep-vcs

  Clone the stable provisioning repository. Don’t forget to specify the last stable version branch 
  with the ``--branch`` option.

  .. code-block:: bash

    $ git clone git@github.com:open-orchestra/open-orchestra-provision.git --branch=1.0

Override the dns redirection
----------------------------

In the ``/etc/hosts`` file of your computer add the following lines:

.. code-block:: text

    192.168.33.10   admin.openorchestra.dev
    192.168.33.10   demo.openorchestra.dev
    192.168.33.10   media.openorchestra.dev

    192.168.33.11   admin.openorchestra.stable
    192.168.33.11   demo.openorchestra.stable
    192.168.33.11   media.openorchestra.stable

You should follow the same steps to install each versions :

* Install roles from ansible-galaxy
* Launch the box
* Install the assets
* Load the fixtures

Install roles from ansible-galaxy
---------------------------------

Go into ``open-orchestra-provisioning`` directory and install roles needed to launch the box:

.. code-block:: bash

    $ ansible-galaxy install --role-file=galaxy.yml

Launch the box
--------------

In the ``open-orchestra`` directory, when you launch the box, it will take some time to:

* Import the base box
* Launch it
* Run all the provisioning scripts

.. code-block:: bash

    $ vagrant up

Install the assets
------------------

We are using npm to manage some server side javascript libraries and bower to manage the client side libraries.

Connect to the vagrant box using ``vagrant ssh``

Finalise the ``composer`` installation in each project:

.. code-block:: bash

    $ cd /var/www/openorchestra && composer run-script post-install-cmd
    $ cd /var/www/front-openorchestra && composer run-script post-install-cmd
    $ cd /var/www/media-openorchestra && composer run-script post-install-cmd

Then go in the Back Office project directory inside the box:

.. code-block:: bash

    $ cd /var/www/openorchestra

Launch the grunt command to generate all assets:

.. code-block:: bash

    $ ./bin/grunt

Load the fixtures
-----------------

In the symfony project directory ``/var/www/openorchestra`` you can load the fixtures provided:

.. code-block:: bash

    $ php app/console doctrine:mongo:fixture:load --env=dev

Result
------

Master version
~~~~~~~~~~~~~~

You can log on http://admin.openorchestra.dev/app_dev.php/login with username=admin and
password=admin for the CMS and see the result on http://demo.openorchestra.dev/app_dev.php.

All the images will be visible on the http://media.openorchestra.dev/app_dev.php url.

Stable version
~~~~~~~~~~~~~~

You can log on http://admin.openorchestra.stable/app_dev.php/login with username=admin and
password=admin for the CMS and see the result on http://demo.openorchestra.stable/app_dev.php.

All the images will be visible on the http://media.openorchestra.stable/app_dev.php url.

.. _`Download Composer`: https://getcomposer.org/download/
.. _`Ansible installation documentation`: http://docs.ansible.com/ansible/intro_installation.html
