=============
FieldTypeType
=============


The FieldTypeType form is used to manage field type in back office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_field_type                                    |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | FieldTypeType                                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |  * prototype_data                                |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              | FieldTypeTypeSubscriber                          |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * fieldId        (text)                          |
|                                   | * labels         (oo_translated_value_collection)|
|                                   | * type           (choice)                        |
|                                   | * listable       (checkbox)                      |
|                                   | * translatable   (checkbox)                      |
|                                   | * searchable     (checkbox)                      |
|                                   | * orderable      (checkbox)                      |
|                                   | * orderDirection (choice)                        |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options:
========

 **prototype_data**

 ..

   **type**: string| array |Closure **default**: null


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: FieldType

 **label**

 ..

    **type**: string **default**: open_orchestra_backoffice.form.field_type.label