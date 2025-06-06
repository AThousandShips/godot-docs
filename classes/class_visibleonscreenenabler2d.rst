:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisibleOnScreenEnabler2D.xml.

.. _class_VisibleOnScreenEnabler2D:

VisibleOnScreenEnabler2D
========================

**Inherits:** :ref:`VisibleOnScreenNotifier2D<class_VisibleOnScreenNotifier2D>` **<** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A rectangular region of 2D space that, when visible on screen, enables a target node.

.. rst-class:: classref-introduction-group

Description
-----------

**VisibleOnScreenEnabler2D** contains a rectangular region of 2D space and a target node. The target node will be automatically enabled (via its :ref:`Node.process_mode<class_Node_property_process_mode>` property) when any part of this region becomes visible on the screen, and automatically disabled otherwise. This can for example be used to activate enemies only when the player approaches them.

See :ref:`VisibleOnScreenNotifier2D<class_VisibleOnScreenNotifier2D>` if you only want to be notified when the region is visible on screen.

\ **Note:** **VisibleOnScreenEnabler2D** uses the render culling code to determine whether it's visible on screen, so it won't function unless :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` is set to ``true``.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------------------------------------+-----------------------------------------------------------------------------------+--------------------+
   | :ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>` | :ref:`enable_mode<class_VisibleOnScreenEnabler2D_property_enable_mode>`           | ``0``              |
   +-------------------------------------------------------------+-----------------------------------------------------------------------------------+--------------------+
   | :ref:`NodePath<class_NodePath>`                             | :ref:`enable_node_path<class_VisibleOnScreenEnabler2D_property_enable_node_path>` | ``NodePath("..")`` |
   +-------------------------------------------------------------+-----------------------------------------------------------------------------------+--------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_VisibleOnScreenEnabler2D_EnableMode:

.. rst-class:: classref-enumeration

enum **EnableMode**: :ref:`🔗<enum_VisibleOnScreenEnabler2D_EnableMode>`

.. _class_VisibleOnScreenEnabler2D_constant_ENABLE_MODE_INHERIT:

.. rst-class:: classref-enumeration-constant

:ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>` **ENABLE_MODE_INHERIT** = ``0``

Corresponds to :ref:`Node.PROCESS_MODE_INHERIT<class_Node_constant_PROCESS_MODE_INHERIT>`.

.. _class_VisibleOnScreenEnabler2D_constant_ENABLE_MODE_ALWAYS:

.. rst-class:: classref-enumeration-constant

:ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>` **ENABLE_MODE_ALWAYS** = ``1``

Corresponds to :ref:`Node.PROCESS_MODE_ALWAYS<class_Node_constant_PROCESS_MODE_ALWAYS>`.

.. _class_VisibleOnScreenEnabler2D_constant_ENABLE_MODE_WHEN_PAUSED:

.. rst-class:: classref-enumeration-constant

:ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>` **ENABLE_MODE_WHEN_PAUSED** = ``2``

Corresponds to :ref:`Node.PROCESS_MODE_WHEN_PAUSED<class_Node_constant_PROCESS_MODE_WHEN_PAUSED>`.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisibleOnScreenEnabler2D_property_enable_mode:

.. rst-class:: classref-property

:ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>` **enable_mode** = ``0`` :ref:`🔗<class_VisibleOnScreenEnabler2D_property_enable_mode>`

.. rst-class:: classref-property-setget

- |void| **set_enable_mode**\ (\ value\: :ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>`\ )
- :ref:`EnableMode<enum_VisibleOnScreenEnabler2D_EnableMode>` **get_enable_mode**\ (\ )

Determines how the target node is enabled. Corresponds to :ref:`ProcessMode<enum_Node_ProcessMode>`. When the node is disabled, it always uses :ref:`Node.PROCESS_MODE_DISABLED<class_Node_constant_PROCESS_MODE_DISABLED>`.

.. rst-class:: classref-item-separator

----

.. _class_VisibleOnScreenEnabler2D_property_enable_node_path:

.. rst-class:: classref-property

:ref:`NodePath<class_NodePath>` **enable_node_path** = ``NodePath("..")`` :ref:`🔗<class_VisibleOnScreenEnabler2D_property_enable_node_path>`

.. rst-class:: classref-property-setget

- |void| **set_enable_node_path**\ (\ value\: :ref:`NodePath<class_NodePath>`\ )
- :ref:`NodePath<class_NodePath>` **get_enable_node_path**\ (\ )

The path to the target node, relative to the **VisibleOnScreenEnabler2D**. The target node is cached; it's only assigned when setting this property (if the **VisibleOnScreenEnabler2D** is inside the scene tree) and every time the **VisibleOnScreenEnabler2D** enters the scene tree. If the path is empty, no node will be affected. If the path is invalid, an error is also generated.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
