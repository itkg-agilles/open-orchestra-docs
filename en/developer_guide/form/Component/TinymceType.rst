===========
TinymceType
===========


The TinymceType form is used to create Tinymce field.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_tinymce                        |
+-----------------------------------+-----------------------------------+
| **Class**                         | AreaType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       | * inherited options FormType      |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **View transformer**              | BBcodeToHtmlTransformer           |
|                                   |                                   |
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: array **default**: array('class' => 'tinymce')