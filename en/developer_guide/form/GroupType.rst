=========
GroupType
=========


The GroupType form is used to contribute a group in Back Office.

+-----------------------------------+-----------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle           |
+-----------------------------------+-----------------------------------------+
| **Name**                          | oo_group                                |
+-----------------------------------+-----------------------------------------+
| **Class**                         | GroupType                               |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Parent type**                   | FormType                                |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Options**                       |  * inherited options FormType           |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Fields** (name, type)           | * name  (text)                          |
|                                   | * labels(oo_translated_value_collection)|
|                                   | * site  (oo_group_site_choice)          |
|                                   | * roles (oo_role_choice)                |
+-----------------------------------+-----------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: Group