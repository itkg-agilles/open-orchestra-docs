==============
NodeChoiceType
==============


The NodeChoiceType form is used to create field choice.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_operator_choice                |
+-----------------------------------+-----------------------------------+
| **Class**                         | NodeChoiceType                    |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | ChoiceType                        |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options ChoiceType   |
|                                   |  * constraints                    |
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/choice.html>`_


Options
=======

 **constraints**

 ..

   **type**: mixed **default**: NotBlank

Overridden Options
==================

 **choices**

 ..

   **type**: array **default**: array()

 **empty_data**

 ..

   **type**: mixed **default**: ContentRepositoryInterface::CHOICE_AND