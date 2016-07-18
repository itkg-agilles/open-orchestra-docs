=============
ApiClientType
=============


The ApiClientType form is used to create a workflow role in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_api_client                                          |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | ApiClientType                                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * name    (text)                                 |
|                                   | * trusted (checkbox)                             |
|                                   | * roles   (oo_role_choice)                       |
|                                   | * key     (text)                                 |
|                                   | * secret  (text)                                 |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options:
========



Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: ApiClient