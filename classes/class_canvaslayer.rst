:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/CanvasLayer.xml.

.. _class_CanvasLayer:

CanvasLayer
===========

**Inherits:** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`ParallaxBackground<class_ParallaxBackground>`

A node used for independent rendering of objects within a 2D scene.

.. rst-class:: classref-introduction-group

Description
-----------

:ref:`CanvasItem<class_CanvasItem>`-derived nodes that are direct or indirect children of a **CanvasLayer** will be drawn in that layer. The layer is a numeric index that defines the draw order. The default 2D scene renders with index ``0``, so a **CanvasLayer** with index ``-1`` will be drawn below, and a **CanvasLayer** with index ``1`` will be drawn above. This order will hold regardless of the :ref:`CanvasItem.z_index<class_CanvasItem_property_z_index>` of the nodes within each layer.

\ **CanvasLayer**\ s can be hidden and they can also optionally follow the viewport. This makes them useful for HUDs like health bar overlays (on layers ``1`` and higher) or backgrounds (on layers ``-1`` and lower).

\ **Note:** Embedded :ref:`Window<class_Window>`\ s are placed on layer ``1024``. :ref:`CanvasItem<class_CanvasItem>`\ s on layers ``1025`` and higher appear in front of embedded windows.

\ **Note:** Each **CanvasLayer** is drawn on one specific :ref:`Viewport<class_Viewport>` and cannot be shared between multiple :ref:`Viewport<class_Viewport>`\ s, see :ref:`custom_viewport<class_CanvasLayer_property_custom_viewport>`. When using multiple :ref:`Viewport<class_Viewport>`\ s, for example in a split-screen game, you need to create an individual **CanvasLayer** for each :ref:`Viewport<class_Viewport>` you want it to be drawn on.

.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`Viewport and canvas transforms <../tutorials/2d/2d_transforms>`

- :doc:`Canvas layers <../tutorials/2d/canvas_layers>`

- `2D Dodge The Creeps Demo <https://godotengine.org/asset-library/asset/2712>`__

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`Node<class_Node>`               | :ref:`custom_viewport<class_CanvasLayer_property_custom_viewport>`                 |                                   |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`follow_viewport_enabled<class_CanvasLayer_property_follow_viewport_enabled>` | ``false``                         |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`float<class_float>`             | :ref:`follow_viewport_scale<class_CanvasLayer_property_follow_viewport_scale>`     | ``1.0``                           |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`int<class_int>`                 | :ref:`layer<class_CanvasLayer_property_layer>`                                     | ``1``                             |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`Vector2<class_Vector2>`         | :ref:`offset<class_CanvasLayer_property_offset>`                                   | ``Vector2(0, 0)``                 |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`float<class_float>`             | :ref:`rotation<class_CanvasLayer_property_rotation>`                               | ``0.0``                           |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`Vector2<class_Vector2>`         | :ref:`scale<class_CanvasLayer_property_scale>`                                     | ``Vector2(1, 1)``                 |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`Transform2D<class_Transform2D>` | :ref:`transform<class_CanvasLayer_property_transform>`                             | ``Transform2D(1, 0, 0, 1, 0, 0)`` |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`visible<class_CanvasLayer_property_visible>`                                 | ``true``                          |
   +---------------------------------------+------------------------------------------------------------------------------------+-----------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`RID<class_RID>`                 | :ref:`get_canvas<class_CanvasLayer_method_get_canvas>`\ (\ ) |const|                   |
   +---------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`Transform2D<class_Transform2D>` | :ref:`get_final_transform<class_CanvasLayer_method_get_final_transform>`\ (\ ) |const| |
   +---------------------------------------+----------------------------------------------------------------------------------------+
   | |void|                                | :ref:`hide<class_CanvasLayer_method_hide>`\ (\ )                                       |
   +---------------------------------------+----------------------------------------------------------------------------------------+
   | |void|                                | :ref:`show<class_CanvasLayer_method_show>`\ (\ )                                       |
   +---------------------------------------+----------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_CanvasLayer_signal_visibility_changed:

.. rst-class:: classref-signal

**visibility_changed**\ (\ ) :ref:`🔗<class_CanvasLayer_signal_visibility_changed>`

Emitted when visibility of the layer is changed. See :ref:`visible<class_CanvasLayer_property_visible>`.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_CanvasLayer_property_custom_viewport:

.. rst-class:: classref-property

:ref:`Node<class_Node>` **custom_viewport** :ref:`🔗<class_CanvasLayer_property_custom_viewport>`

.. rst-class:: classref-property-setget

- |void| **set_custom_viewport**\ (\ value\: :ref:`Node<class_Node>`\ )
- :ref:`Node<class_Node>` **get_custom_viewport**\ (\ )

The custom :ref:`Viewport<class_Viewport>` node assigned to the **CanvasLayer**. If ``null``, uses the default viewport instead.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_follow_viewport_enabled:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **follow_viewport_enabled** = ``false`` :ref:`🔗<class_CanvasLayer_property_follow_viewport_enabled>`

.. rst-class:: classref-property-setget

- |void| **set_follow_viewport**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_following_viewport**\ (\ )

If enabled, the **CanvasLayer** maintains its position in world space. If disabled, the **CanvasLayer** stays in a fixed position on the screen.

Together with :ref:`follow_viewport_scale<class_CanvasLayer_property_follow_viewport_scale>`, this can be used for a pseudo-3D effect.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_follow_viewport_scale:

.. rst-class:: classref-property

:ref:`float<class_float>` **follow_viewport_scale** = ``1.0`` :ref:`🔗<class_CanvasLayer_property_follow_viewport_scale>`

.. rst-class:: classref-property-setget

- |void| **set_follow_viewport_scale**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_follow_viewport_scale**\ (\ )

Scales the layer when using :ref:`follow_viewport_enabled<class_CanvasLayer_property_follow_viewport_enabled>`. Layers moving into the foreground should have increasing scales, while layers moving into the background should have decreasing scales.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_layer:

.. rst-class:: classref-property

:ref:`int<class_int>` **layer** = ``1`` :ref:`🔗<class_CanvasLayer_property_layer>`

.. rst-class:: classref-property-setget

- |void| **set_layer**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_layer**\ (\ )

Layer index for draw order. Lower values are drawn behind higher values.

\ **Note:** If multiple CanvasLayers have the same layer index, :ref:`CanvasItem<class_CanvasItem>` children of one CanvasLayer are drawn behind the :ref:`CanvasItem<class_CanvasItem>` children of the other CanvasLayer. Which CanvasLayer is drawn in front is non-deterministic.

\ **Note:** The layer index should be between :ref:`RenderingServer.CANVAS_LAYER_MIN<class_RenderingServer_constant_CANVAS_LAYER_MIN>` and :ref:`RenderingServer.CANVAS_LAYER_MAX<class_RenderingServer_constant_CANVAS_LAYER_MAX>` (inclusive). Any other value will wrap around.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_offset:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **offset** = ``Vector2(0, 0)`` :ref:`🔗<class_CanvasLayer_property_offset>`

.. rst-class:: classref-property-setget

- |void| **set_offset**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_offset**\ (\ )

The layer's base offset.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_rotation:

.. rst-class:: classref-property

:ref:`float<class_float>` **rotation** = ``0.0`` :ref:`🔗<class_CanvasLayer_property_rotation>`

.. rst-class:: classref-property-setget

- |void| **set_rotation**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_rotation**\ (\ )

The layer's rotation in radians.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_scale:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **scale** = ``Vector2(1, 1)`` :ref:`🔗<class_CanvasLayer_property_scale>`

.. rst-class:: classref-property-setget

- |void| **set_scale**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_scale**\ (\ )

The layer's scale.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_transform:

.. rst-class:: classref-property

:ref:`Transform2D<class_Transform2D>` **transform** = ``Transform2D(1, 0, 0, 1, 0, 0)`` :ref:`🔗<class_CanvasLayer_property_transform>`

.. rst-class:: classref-property-setget

- |void| **set_transform**\ (\ value\: :ref:`Transform2D<class_Transform2D>`\ )
- :ref:`Transform2D<class_Transform2D>` **get_transform**\ (\ )

The layer's transform.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_property_visible:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **visible** = ``true`` :ref:`🔗<class_CanvasLayer_property_visible>`

.. rst-class:: classref-property-setget

- |void| **set_visible**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_visible**\ (\ )

If ``false``, any :ref:`CanvasItem<class_CanvasItem>` under this **CanvasLayer** will be hidden.

Unlike :ref:`CanvasItem.visible<class_CanvasItem_property_visible>`, visibility of a **CanvasLayer** isn't propagated to underlying layers.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_CanvasLayer_method_get_canvas:

.. rst-class:: classref-method

:ref:`RID<class_RID>` **get_canvas**\ (\ ) |const| :ref:`🔗<class_CanvasLayer_method_get_canvas>`

Returns the RID of the canvas used by this layer.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_method_get_final_transform:

.. rst-class:: classref-method

:ref:`Transform2D<class_Transform2D>` **get_final_transform**\ (\ ) |const| :ref:`🔗<class_CanvasLayer_method_get_final_transform>`

Returns the transform from the **CanvasLayer**\ s coordinate system to the :ref:`Viewport<class_Viewport>`\ s coordinate system.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_method_hide:

.. rst-class:: classref-method

|void| **hide**\ (\ ) :ref:`🔗<class_CanvasLayer_method_hide>`

Hides any :ref:`CanvasItem<class_CanvasItem>` under this **CanvasLayer**. This is equivalent to setting :ref:`visible<class_CanvasLayer_property_visible>` to ``false``.

.. rst-class:: classref-item-separator

----

.. _class_CanvasLayer_method_show:

.. rst-class:: classref-method

|void| **show**\ (\ ) :ref:`🔗<class_CanvasLayer_method_show>`

Shows any :ref:`CanvasItem<class_CanvasItem>` under this **CanvasLayer**. This is equivalent to setting :ref:`visible<class_CanvasLayer_property_visible>` to ``true``.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
