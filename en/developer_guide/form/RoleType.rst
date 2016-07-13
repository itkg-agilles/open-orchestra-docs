========
RoleType
========


The RoleType form is used to create a workflow role in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_role                                          |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | RoleType                                         |
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
| **Fields** (name, type)           | * name         (text)                            |
|                                   | * descriptions (oo_translated_value_collection)  |
|                                   | * fromStatus   (oo_status_choice)                |
|                                   | * toStatus     (oo_status_choice)                |
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

   **type**: string **default**: Role