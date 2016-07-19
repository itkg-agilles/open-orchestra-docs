==========
StatusType
==========


The StatusType form is used to create a workflow status in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_status                                        |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | StatusType                                       |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * name         (text)                            |
|                                   | * published    (text)                            |
|                                   | * initial      (oo_status_choice)                |
|                                   | * labels       (oo_translated_value_collection)  |
|                                   | * displayColor (orchestra_color_choice)          |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: Status