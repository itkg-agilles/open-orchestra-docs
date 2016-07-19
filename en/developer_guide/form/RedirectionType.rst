===============
RedirectionType
===============


The RedirectionType form is used to create a redirection in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_redirection                                   |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | RedirectionType                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              | RedirectionTypeSubscriber                        |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * siteId       (oo_site_choice)                  |
|                                   | * locale       (orchestra_language)              |
|                                   | * routePattern (text)                            |
|                                   | * nodeId       (oo_node_choice)                  |
|                                   | * url          (text)                            |
|                                   | * permanent    (checkbox)                        |
+-----------------------------------+--------------------------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Overridden Options
==================

 **data_class**

 ..

   **type**: string **default**: `Redirection <https://github.com/open-orchestra/open-orchestra-model-bundle/blob/3e1d29dcff1fa2fa8425c28d92eb11ac37d7d330/ModelBundle/Document/Redirection.php>`_