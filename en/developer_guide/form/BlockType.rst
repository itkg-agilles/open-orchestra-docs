=========
BlockType
=========


The BlockType form is used to parameter a block in Back Office.

+-----------------------------------+-----------------------------------+
| **Bundle**                        | OpenOrchestraBackofficeBundle     |
+-----------------------------------+-----------------------------------+
| **Name**                          | oo_block                          |
+-----------------------------------+-----------------------------------+
| **Class**                         | BlockType                         |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Parent type**                   | FormType                          |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Options**                       |  * inherited options FormType     |
|                                   |  * blockPosition                  |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Event subscriber**              | BlockTypeSubscriber               |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **View transformer**              | BlockToArrayTransformer           |
|                                   |                                   |
+-----------------------------------+-----------------------------------+
| **Fields** (name, type)           | * label  (text)                   |
|                                   | * class  (text)                   |
|                                   | * id     (text)                   |
|                                   | * maxAge (integer)                |
+-----------------------------------+-----------------------------------+


Inherited Options:
==================

 Options inherit from the `FormType <http://symfony.com/doc/current/reference/forms/types/form.html>`_


Options:
========

 **blockPosition**

 ..

    **type**: integer **default**: 0
    Block position is the position of block in area


Overridden Options
==================
 
 **data_class**
 
 ..

   **type**: string **default**: null