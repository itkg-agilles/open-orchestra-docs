===============
ContentTypeType
===============


The ContentTypeType form is used to contribute a content type in Back Office.

+-----------------------------------+-----------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle           |
+-----------------------------------+-----------------------------------------+
| **Name**                          | oo_content_type                         |
+-----------------------------------+-----------------------------------------+
| **Class**                         | ContentTypeType                         |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Parent type**                   | FormType                                |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Options**                       |  * inherited options FormType           |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Event subscriber**              | ContentTypeTypeSubscriber               |
|                                   |                                         |
+-----------------------------------+-----------------------------------------+
| **Fields** (name, type)           | * contentTypeId        (text)           |
|                                   | * names (oo_translated_value_collection)|
|                                   | * template (text)                       |
|                                   | * linkedToSite (checkbox)               |
|                                   | * defaultListable (collection)          |
|                                   | * fields (collection)                   |
+-----------------------------------+-----------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: ContentType