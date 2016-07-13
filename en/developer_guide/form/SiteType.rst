========
SiteType
========


The SiteType form is used to create a web site in Back Office.

+-----------------------------------+--------------------------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle                    |
+-----------------------------------+--------------------------------------------------+
| **Name**                          | oo_site                                          |
+-----------------------------------+--------------------------------------------------+
| **Class**                         | SiteType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Parent type**                   | FormType                                         |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Options**                       |  * inherited options FormType                    |
|                                   |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Event subscriber**              | WebSiteSubscriber                                |
|                                   | WebSiteNodeTemplateSubscriber                    |
+-----------------------------------+--------------------------------------------------+
| **View transformer**              |                                                  |
|                                   |                                                  |
+-----------------------------------+--------------------------------------------------+
| **Fields** (name, type)           | * name    (text)                                 |
|                                   | * siteId  (text)                                 |
|                                   | * aliases (collection)                           |
|                                   | * blocks  (oo_block_choice)                      |
|                                   | * theme   (oo_site_theme_choice)                 |
|                                   | * sitemap_changefreq (orchestra_frequence_choice)|
|                                   | * sitemap_priority (percent)                     |
|                                   | * metaKeywords     (oo_multi_languages_text)     |
|                                   | * metaDescriptions (oo_multi_languages_text)     |
|                                   | * metaIndex  (checkbox)                          |
|                                   | * metaFollow (checkbox)                          |
|                                   | * robotsTxt  (textarea)                          |
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

   **type**: string **default**: Site