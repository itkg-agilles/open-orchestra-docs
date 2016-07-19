============
TemplateType
============


The TemplateType form is used to manage template in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_template                                      |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | TemplateType                                     |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              | AreaCollectionSubscriber                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * name        (text)                             |
|                                   | * language    (orchestra_language)               |
|                                   | * boDirection (orchestra_direction)              |
|                                   | * templateId  (hidden)                           |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: Template