===========
ContentType
===========


The ContentType form is used to parameter a content type in Back Office.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_content                        |
+-----------------------------------+-----------------------------------+
| **Class**                         | ContentType                       |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options FormType     |
|                                   |                                   |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Event subscriber**              | ContentTypeSubscriber             |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **View transformer**              |                                   |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Fields** (name, type)           | * name        (text)              |
|                                   | * keywords    (oo_keywords_choice)|
|                                   | * linkedToSite(checkbox)          |
|                                   |                                   |
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

   **type**: string **default**: Content