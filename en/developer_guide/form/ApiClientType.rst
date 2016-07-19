=============
ApiClientType
=============


The ApiClientType form is used to create API key access in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_api_client                                    |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | ApiClientType                                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
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


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: ApiClient