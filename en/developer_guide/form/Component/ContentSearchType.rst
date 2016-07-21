=================
ContentSearchType
=================


The ContentSearchType form is used to create content search field.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_content_search                                |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | ContentSearchType                                |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |  * refresh                                       |
|                                   |  * authorize_new                                 |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              | ContentSearchSubscriber                          |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * contentType (oo_content_type_choice)           |
|                                   | * choiceType  (oo_operator_choice)               |
|                                   | * keywords    (oo_keywords_choice)               |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options
=======

 **refresh**

 ..

   **type**: boolean **default**: false

 **authorize_new**

 ..

   **type**: string **default**: null