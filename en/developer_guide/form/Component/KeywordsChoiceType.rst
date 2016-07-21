==================
KeywordsChoiceType
==================


The KeywordsChoiceType form is used to manage keywords.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_keywords_choice                               |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | KeywordsChoiceType                               |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | TextType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options TextType                    |
|                                   |  * attr                                          |
|                                   |  * name                                          |
|                                   |  * new_attr                                      |
|                                   |  * is_condition                                  |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              | CsvToReferenceKeywordTransformer                 |
|                                   | ConditionToReferenceKeywordTransformer           |
+-----------------------------------+--------------------------------------------------+

Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/text.html>`_


Options
=======

 **attr**

 ..

   **type**: string | array | Closure **default**: array()

 **name**

 ..

   **type**: string **default**: ''

 **new_attr**

 ..

   **type**: string | array | Closure **default**: array()

 **name**

 ..

   **type**: boolean **default**: false