========
AreaType
========


The AreaType form is used to parameter a area in Back Office.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_area                           |
+-----------------------------------+-----------------------------------+
| **Class**                         | AreaType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options FormType     |
|                                   |                                   |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Event subscriber**              | AreaCollectionSubscriber          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **View transformer**              | HtmlElementTransformer            |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Fields** (name, type)           | * label       (text)              |
|                                   | * areaId      (text)              |
|                                   | * htmlClass   (text)              |
|                                   | * boDirection (choice)            |
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options:
========



Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: Area