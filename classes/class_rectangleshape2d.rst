:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/RectangleShape2D.xml.

.. _class_RectangleShape2D:

RectangleShape2D
================

**Inherits:** :ref:`Shape2D<class_Shape2D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A 2D rectangle shape used for physics collision.

.. rst-class:: classref-introduction-group

Description
-----------

A 2D rectangle shape, intended for use in physics. Usually used to provide a shape for a :ref:`CollisionShape2D<class_CollisionShape2D>`.

\ **Performance:** **RectangleShape2D** is fast to check collisions against. It is faster than :ref:`CapsuleShape2D<class_CapsuleShape2D>`, but slower than :ref:`CircleShape2D<class_CircleShape2D>`.

.. rst-class:: classref-introduction-group

Tutorials
---------

- `2D Pong Demo <https://godotengine.org/asset-library/asset/2728>`__

- `2D Kinematic Character Demo <https://godotengine.org/asset-library/asset/2719>`__

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------+---------------------------------------------------+---------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`size<class_RectangleShape2D_property_size>` | ``Vector2(20, 20)`` |
   +-------------------------------+---------------------------------------------------+---------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_RectangleShape2D_property_size:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **size** = ``Vector2(20, 20)`` :ref:`🔗<class_RectangleShape2D_property_size>`

.. rst-class:: classref-property-setget

- |void| **set_size**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_size**\ (\ )

The rectangle's width and height.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
