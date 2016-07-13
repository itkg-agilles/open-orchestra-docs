========
NodeType
========


The NodeType form is used to contribute a node in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_node                                          |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | NodeType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              | BoDirectionChildrenSubscriber                    |
|                                   | NodeTemplateSelectionSubscriber                  |
|                                   | NodeThemeSelectionSubscriber                     |
|                                   | AreaCollectionSubscriber                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * name               (text)                      |
|                                   | * boLabel            (text)                      |
|                                   | * routePattern       (text)                      |
|                                   | * scheme             (choice)                    |
|                                   | * sitemap_changefreq (orchestra_frequence_choice)|
|                                   | * sitemap_priority   (percent)                   |
|                                   | * theme              (oo_theme_choice)           |
|                                   | * inMenu             (checkbox)                  |
|                                   | * inFooter           (checkbox)                  |
|                                   | * metaKeywords       (text)                      |
|                                   | * metaDescription    (text)                      |
|                                   | * metaIndex          (checkbox)                  |
|                                   | * metaFollow         (checkbox)                  |
|                                   | * nodeId             (hidden)                    |
|                                   | * role               (oo_front_role_choice)      |
|                                   | * maxAge             (integer)                   |
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

   **type**: string **default**: Node