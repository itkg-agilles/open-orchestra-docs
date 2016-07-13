=============
SiteAliasType
=============


The SiteAliasType form is used to create a alias in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_site_alias                                    |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | SiteAliasType                                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * scheme   (choice)                              |
|                                   | * domain   (text)                                |
|                                   | * language (orchestra_language)                  |
|                                   | * prefix   (text)                                |
|                                   | * main     (checkbox)                            |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options:
========



Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: SiteAlias