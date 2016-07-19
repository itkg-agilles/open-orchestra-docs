===============
FieldOptionType
===============


The FieldOptionType form is used to manage field option in Back Office.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_field_option                   |
+-----------------------------------+-----------------------------------+
| **Class**                         | FieldOptionType                   |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options FormType     |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Event subscriber**              | FieldOptionTypeSubscribe          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Fields** (name, type)           | * key (hidden)                    |
|                                   |                                   |
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: FieldOption

 **label**

 ..

    **type**: string **default**: open_orchestra_backoffice.form.field_option.label