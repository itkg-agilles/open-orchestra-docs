Improve Vagrant with KVM
========================

Context
-------

A simple installation of `vagrant`_ will be working with `virtualbox`_. In some cases, you
will notice that `virtualbox`_ is not the faster solution on the market. `KVM`_ can be a good
alternative for the virtualization on your own computer.

Basic installation
------------------

KVM installation
~~~~~~~~~~~~~~~~

You need to install all the packages for the vagrant plugin, and to allow `KVM`_ to run.

.. code-block:: bash

    $ aptitude install libxslt-dev libxml2-dev libvirt-dev zlib1g-dev qemu-utils libvirt-dev libvirt-bin qemu-kvm
    $ gem install ruby-libvirt -v '0.6.0'

Change images location (optional)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The following step is optional but you may want to change the ``libvirt`` default images storage location which is set
to ``/var/lib/libvirt/images`` to somewhere else in order to save space in the ``/var`` directory especially if ``/var``
is on a dedicated partition.

.. code-block:: bash

    $ cd /etc/libvirt/storage
    $ virsh pool-edit default

Now, you must change the old path to images in the ``path`` tag to the new one and save.

.. code-block:: xml

    <pool type='dir'>
        <name>default</name>
        <uuid>8712914f-3330-474f-8766-096761b1c3c2</uuid>
        <capacity unit='bytes'>463178629120</capacity>
        <allocation unit='bytes'>111961907200</allocation>
        <available unit='bytes'>351216721920</available>
        <source>
        </source>
        <target>
        <path>/your/new/path/to/images</path>
        <permissions>
          <mode>0755</mode>
          <owner>-1</owner>
          <group>-1</group>
        </permissions>
        </target>
    </pool>

The following message is displayed:

.. code-block:: bash

    Pool default XML configuration edited.

Then you have to restart the ``libvirt`` daemon.

.. code-block:: bash

    $ /etc/init.d/libvirtd restart

Vagrant plugin installation
~~~~~~~~~~~~~~~~~~~~~~~~~~~

The `libvirt`_ plugin should be added to vagrant

.. code-block:: bash

    $ vagrant plugin install vagrant-libvirt

Launch the box
~~~~~~~~~~~~~~

Once those installations have been performed, if you have imported the right base box, you could launch
your box with :

.. code-block:: bash

    $ vagrant up --provider=libvirt

You can check that your box is running on `qemu`_ instead of `virtualbox`_.

Mutate a box
------------

If you do not find a box created for libvirt, you can convert an existing one by using the `vagrant`_
`mutate`_ plugin.

Plugin installation
~~~~~~~~~~~~~~~~~~~

Directly install the plugin

.. code-block:: bash

    $ vagrant plugin install vagrant-mutate

Convert your box
~~~~~~~~~~~~~~~~

We suppose that you have already registered the ``bento/debian8.2`` base box.

.. code-block:: bash

    $ vagrant mutate bento/debian-8.2 libvirt

You can now launch the box as done before.

.. _`vagrant`: https://www.vagrantup.com/
.. _`qemu`: http://wiki.qemu.org/Main_Page
.. _`virtualbox`: https://www.virtualbox.org/
.. _`KVM`: http://www.linux-kvm.org/page/Main_Page
.. _`mutate`: https://github.com/sciurus/vagrant-mutate
.. _`libvirt`: https://github.com/pradels/vagrant-libvirt
