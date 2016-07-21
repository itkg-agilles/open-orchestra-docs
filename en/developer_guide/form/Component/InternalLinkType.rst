================
InternalLinkType
================


The InternalLinkType form is used to manage internal link.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_internal_link                                 |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | InternalLinkType                                 |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options CheckboxType                |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * label         (text)                           |
|                                   | * nodeId        (oo_node_choice)                 |
|                                   | * contentSearch (oo_content_search)              |
|                                   | * site          (oo_site_site_alias)             |
|                                   | * query         (text)                           |
+-----------------------------------+--------------------------------------------------+

Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_