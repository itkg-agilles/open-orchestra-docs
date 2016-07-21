=================
SiteSiteAliasType
=================


The SiteSiteAliasType form is used to create a site alias.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_site_site_alias                |
+-----------------------------------+-----------------------------------+
| **Class**                         | SiteSiteAliasType                 |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options FormType     |
|                                   |  * refresh                        |
|                                   |  * attr                           |
+-----------------------------------+-----------------------------------+
| **Event subscriber**              | SiteSubscriber                    |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Fields** (name, type)           | * siteId (oo_site_choice)         |
|                                   |                                   |
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options
=======

 **refresh**

 ..

   **type**: boolean **default**: false

 **attr**

 ..

   **type**: array **default**: array()