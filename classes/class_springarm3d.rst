:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/SpringArm3D.xml.

.. _class_SpringArm3D:

SpringArm3D
===========

**Inherits:** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A 3D raycast that dynamically moves its children near the collision point.

.. rst-class:: classref-introduction-group

Description
-----------

**SpringArm3D** casts a ray or a shape along its Z axis and moves all its direct children to the collision point, with an optional margin. This is useful for 3rd person cameras that move closer to the player when inside a tight space (you may need to exclude the player's collider from the **SpringArm3D**'s collision check).

.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`Third-person camera with spring arm <../tutorials/3d/spring_arm>`

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------+------------------------------------------------------------------+----------+
   | :ref:`int<class_int>`         | :ref:`collision_mask<class_SpringArm3D_property_collision_mask>` | ``1``    |
   +-------------------------------+------------------------------------------------------------------+----------+
   | :ref:`float<class_float>`     | :ref:`margin<class_SpringArm3D_property_margin>`                 | ``0.01`` |
   +-------------------------------+------------------------------------------------------------------+----------+
   | :ref:`Shape3D<class_Shape3D>` | :ref:`shape<class_SpringArm3D_property_shape>`                   |          |
   +-------------------------------+------------------------------------------------------------------+----------+
   | :ref:`float<class_float>`     | :ref:`spring_length<class_SpringArm3D_property_spring_length>`   | ``1.0``  |
   +-------------------------------+------------------------------------------------------------------+----------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------+-------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`add_excluded_object<class_SpringArm3D_method_add_excluded_object>`\ (\ RID\: :ref:`RID<class_RID>`\ )       |
   +---------------------------+-------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`clear_excluded_objects<class_SpringArm3D_method_clear_excluded_objects>`\ (\ )                              |
   +---------------------------+-------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`get_hit_length<class_SpringArm3D_method_get_hit_length>`\ (\ )                                              |
   +---------------------------+-------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`   | :ref:`remove_excluded_object<class_SpringArm3D_method_remove_excluded_object>`\ (\ RID\: :ref:`RID<class_RID>`\ ) |
   +---------------------------+-------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_SpringArm3D_property_collision_mask:

.. rst-class:: classref-property

:ref:`int<class_int>` **collision_mask** = ``1`` :ref:`🔗<class_SpringArm3D_property_collision_mask>`

.. rst-class:: classref-property-setget

- |void| **set_collision_mask**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_collision_mask**\ (\ )

The layers against which the collision check shall be done. See `Collision layers and masks <../tutorials/physics/physics_introduction.html#collision-layers-and-masks>`__ in the documentation for more information.

.. rst-class:: classref-item-separator

----

.. _class_SpringArm3D_property_margin:

.. rst-class:: classref-property

:ref:`float<class_float>` **margin** = ``0.01`` :ref:`🔗<class_SpringArm3D_property_margin>`

.. rst-class:: classref-property-setget

- |void| **set_margin**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_margin**\ (\ )

When the collision check is made, a candidate length for the SpringArm3D is given.

The margin is then subtracted to this length and the translation is applied to the child objects of the SpringArm3D.

This margin is useful for when the SpringArm3D has a :ref:`Camera3D<class_Camera3D>` as a child node: without the margin, the :ref:`Camera3D<class_Camera3D>` would be placed on the exact point of collision, while with the margin the :ref:`Camera3D<class_Camera3D>` would be placed close to the point of collision.

.. rst-class:: classref-item-separator

----

.. _class_SpringArm3D_property_shape:

.. rst-class:: classref-property

:ref:`Shape3D<class_Shape3D>` **shape** :ref:`🔗<class_SpringArm3D_property_shape>`

.. rst-class:: classref-property-setget

- |void| **set_shape**\ (\ value\: :ref:`Shape3D<class_Shape3D>`\ )
- :ref:`Shape3D<class_Shape3D>` **get_shape**\ (\ )

The :ref:`Shape3D<class_Shape3D>` to use for the SpringArm3D.

When the shape is set, the SpringArm3D will cast the :ref:`Shape3D<class_Shape3D>` on its z axis instead of performing a ray cast.

.. rst-class:: classref-item-separator

----

.. _class_SpringArm3D_property_spring_length:

.. rst-class:: classref-property

:ref:`float<class_float>` **spring_length** = ``1.0`` :ref:`🔗<class_SpringArm3D_property_spring_length>`

.. rst-class:: classref-property-setget

- |void| **set_length**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_length**\ (\ )

The maximum extent of the SpringArm3D. This is used as a length for both the ray and the shape cast used internally to calculate the desired position of the SpringArm3D's child nodes.

To know more about how to perform a shape cast or a ray cast, please consult the :ref:`PhysicsDirectSpaceState3D<class_PhysicsDirectSpaceState3D>` documentation.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_SpringArm3D_method_add_excluded_object:

.. rst-class:: classref-method

|void| **add_excluded_object**\ (\ RID\: :ref:`RID<class_RID>`\ ) :ref:`🔗<class_SpringArm3D_method_add_excluded_object>`

Adds the :ref:`PhysicsBody3D<class_PhysicsBody3D>` object with the given :ref:`RID<class_RID>` to the list of :ref:`PhysicsBody3D<class_PhysicsBody3D>` objects excluded from the collision check.

.. rst-class:: classref-item-separator

----

.. _class_SpringArm3D_method_clear_excluded_objects:

.. rst-class:: classref-method

|void| **clear_excluded_objects**\ (\ ) :ref:`🔗<class_SpringArm3D_method_clear_excluded_objects>`

Clears the list of :ref:`PhysicsBody3D<class_PhysicsBody3D>` objects excluded from the collision check.

.. rst-class:: classref-item-separator

----

.. _class_SpringArm3D_method_get_hit_length:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_hit_length**\ (\ ) :ref:`🔗<class_SpringArm3D_method_get_hit_length>`

Returns the spring arm's current length.

.. rst-class:: classref-item-separator

----

.. _class_SpringArm3D_method_remove_excluded_object:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **remove_excluded_object**\ (\ RID\: :ref:`RID<class_RID>`\ ) :ref:`🔗<class_SpringArm3D_method_remove_excluded_object>`

Removes the given :ref:`RID<class_RID>` from the list of :ref:`PhysicsBody3D<class_PhysicsBody3D>` objects excluded from the collision check.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
