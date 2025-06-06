:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisibleOnScreenNotifier2D.xml.

.. _class_VisibleOnScreenNotifier2D:

VisibleOnScreenNotifier2D
=========================

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`VisibleOnScreenEnabler2D<class_VisibleOnScreenEnabler2D>`

A rectangular region of 2D space that detects whether it is visible on screen.

.. rst-class:: classref-introduction-group

Description
-----------

**VisibleOnScreenNotifier2D** represents a rectangular region of 2D space. When any part of this region becomes visible on screen or in a viewport, it will emit a :ref:`screen_entered<class_VisibleOnScreenNotifier2D_signal_screen_entered>` signal, and likewise it will emit a :ref:`screen_exited<class_VisibleOnScreenNotifier2D_signal_screen_exited>` signal when no part of it remains visible.

If you want a node to be enabled automatically when this region is visible on screen, use :ref:`VisibleOnScreenEnabler2D<class_VisibleOnScreenEnabler2D>`.

\ **Note:** **VisibleOnScreenNotifier2D** uses the render culling code to determine whether it's visible on screen, so it won't function unless :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` is set to ``true``.

.. rst-class:: classref-introduction-group

Tutorials
---------

- `2D Dodge The Creeps Demo <https://godotengine.org/asset-library/asset/2712>`__

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------+----------------------------------------------------------------------+-----------------------------+
   | :ref:`Rect2<class_Rect2>` | :ref:`rect<class_VisibleOnScreenNotifier2D_property_rect>`           | ``Rect2(-10, -10, 20, 20)`` |
   +---------------------------+----------------------------------------------------------------------+-----------------------------+
   | :ref:`bool<class_bool>`   | :ref:`show_rect<class_VisibleOnScreenNotifier2D_property_show_rect>` | ``true``                    |
   +---------------------------+----------------------------------------------------------------------+-----------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-------------------------+----------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>` | :ref:`is_on_screen<class_VisibleOnScreenNotifier2D_method_is_on_screen>`\ (\ ) |const| |
   +-------------------------+----------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_VisibleOnScreenNotifier2D_signal_screen_entered:

.. rst-class:: classref-signal

**screen_entered**\ (\ ) :ref:`🔗<class_VisibleOnScreenNotifier2D_signal_screen_entered>`

Emitted when the VisibleOnScreenNotifier2D enters the screen.

.. rst-class:: classref-item-separator

----

.. _class_VisibleOnScreenNotifier2D_signal_screen_exited:

.. rst-class:: classref-signal

**screen_exited**\ (\ ) :ref:`🔗<class_VisibleOnScreenNotifier2D_signal_screen_exited>`

Emitted when the VisibleOnScreenNotifier2D exits the screen.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisibleOnScreenNotifier2D_property_rect:

.. rst-class:: classref-property

:ref:`Rect2<class_Rect2>` **rect** = ``Rect2(-10, -10, 20, 20)`` :ref:`🔗<class_VisibleOnScreenNotifier2D_property_rect>`

.. rst-class:: classref-property-setget

- |void| **set_rect**\ (\ value\: :ref:`Rect2<class_Rect2>`\ )
- :ref:`Rect2<class_Rect2>` **get_rect**\ (\ )

The VisibleOnScreenNotifier2D's bounding rectangle.

.. rst-class:: classref-item-separator

----

.. _class_VisibleOnScreenNotifier2D_property_show_rect:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **show_rect** = ``true`` :ref:`🔗<class_VisibleOnScreenNotifier2D_property_show_rect>`

.. rst-class:: classref-property-setget

- |void| **set_show_rect**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_showing_rect**\ (\ )

If ``true``, shows the rectangle area of :ref:`rect<class_VisibleOnScreenNotifier2D_property_rect>` in the editor with a translucent magenta fill. Unlike changing the visibility of the VisibleOnScreenNotifier2D, this does not affect the screen culling detection.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_VisibleOnScreenNotifier2D_method_is_on_screen:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_on_screen**\ (\ ) |const| :ref:`🔗<class_VisibleOnScreenNotifier2D_method_is_on_screen>`

If ``true``, the bounding rectangle is on the screen.

\ **Note:** It takes one frame for the **VisibleOnScreenNotifier2D**'s visibility to be determined once added to the scene tree, so this method will always return ``false`` right after it is instantiated, before the draw pass.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
