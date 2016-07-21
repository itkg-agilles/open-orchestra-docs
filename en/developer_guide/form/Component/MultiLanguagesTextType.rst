======================
MultiLanguagesTextType
======================


The MultiLanguagesTextType form is used to manage multi language text.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_multi_languages_text                          |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | MultiLanguagesTextType                           |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |  * languages                                     |
|                                   |  * type                                          |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              | DataTransformerInterface                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+

Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options
=======

 **languages**

 ..

   **type**: array **default**: array('en')

 **type**

 ..

   **type**: string **default**: 'text'

Overridden Options
==================

 **label_attr**

 ..

   **type**: array **default**: array('class' => 'translated-value')