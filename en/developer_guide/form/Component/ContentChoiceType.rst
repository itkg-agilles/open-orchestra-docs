=================
ContentChoiceType
=================


The ContentChoiceType form is used to create a content choice field.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_content_choice                 |
+-----------------------------------+-----------------------------------+
| **Class**                         | ContentChoiceType                 |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options FormType     |
|                                   |  * content_search                 |
+-----------------------------------+-----------------------------------+
| **View transformer**              | ReferenceToEmbedTransformer       |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Fields** (name, type)           | * $formTypeName (choice)          |
|                                   | passed as parameter in constructor|
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options
=======

 **content_search**

 ..

   **type**: array **default**: array()