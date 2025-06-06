:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/SkeletonModification2DJiggle.xml.

.. _class_SkeletonModification2DJiggle:

SkeletonModification2DJiggle
============================

**Experimental:** This class may be changed or removed in future versions.

**Inherits:** :ref:`SkeletonModification2D<class_SkeletonModification2D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A modification that jiggles :ref:`Bone2D<class_Bone2D>` nodes as they move towards a target.

.. rst-class:: classref-introduction-group

Description
-----------

This modification moves a series of bones, typically called a bone chain, towards a target. What makes this modification special is that it calculates the velocity and acceleration for each bone in the bone chain, and runs a very light physics-like calculation using the inputted values. This allows the bones to overshoot the target and "jiggle" around. It can be configured to act more like a spring, or sway around like cloth might.

This modification is useful for adding additional motion to things like hair, the edges of clothing, and more. It has several settings to that allow control over how the joint moves when the target moves.

\ **Note:** The Jiggle modifier has ``jiggle_joints``, which are the data objects that hold the data for each joint in the Jiggle chain. This is different from than :ref:`Bone2D<class_Bone2D>` nodes! Jiggle joints hold the data needed for each :ref:`Bone2D<class_Bone2D>` in the bone chain used by the Jiggle modification.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`float<class_float>`       | :ref:`damping<class_SkeletonModification2DJiggle_property_damping>`                                   | ``0.75``          |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`Vector2<class_Vector2>`   | :ref:`gravity<class_SkeletonModification2DJiggle_property_gravity>`                                   | ``Vector2(0, 6)`` |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`int<class_int>`           | :ref:`jiggle_data_chain_length<class_SkeletonModification2DJiggle_property_jiggle_data_chain_length>` | ``0``             |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`float<class_float>`       | :ref:`mass<class_SkeletonModification2DJiggle_property_mass>`                                         | ``0.75``          |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`float<class_float>`       | :ref:`stiffness<class_SkeletonModification2DJiggle_property_stiffness>`                               | ``3.0``           |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`NodePath<class_NodePath>` | :ref:`target_nodepath<class_SkeletonModification2DJiggle_property_target_nodepath>`                   | ``NodePath("")``  |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+
   | :ref:`bool<class_bool>`         | :ref:`use_gravity<class_SkeletonModification2DJiggle_property_use_gravity>`                           | ``false``         |
   +---------------------------------+-------------------------------------------------------------------------------------------------------+-------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`           | :ref:`get_collision_mask<class_SkeletonModification2DJiggle_method_get_collision_mask>`\ (\ ) |const|                                                                                               |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`NodePath<class_NodePath>` | :ref:`get_jiggle_joint_bone2d_node<class_SkeletonModification2DJiggle_method_get_jiggle_joint_bone2d_node>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                        |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`           | :ref:`get_jiggle_joint_bone_index<class_SkeletonModification2DJiggle_method_get_jiggle_joint_bone_index>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                          |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`       | :ref:`get_jiggle_joint_damping<class_SkeletonModification2DJiggle_method_get_jiggle_joint_damping>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                                |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector2<class_Vector2>`   | :ref:`get_jiggle_joint_gravity<class_SkeletonModification2DJiggle_method_get_jiggle_joint_gravity>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                                |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`       | :ref:`get_jiggle_joint_mass<class_SkeletonModification2DJiggle_method_get_jiggle_joint_mass>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                                      |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`         | :ref:`get_jiggle_joint_override<class_SkeletonModification2DJiggle_method_get_jiggle_joint_override>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                              |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`       | :ref:`get_jiggle_joint_stiffness<class_SkeletonModification2DJiggle_method_get_jiggle_joint_stiffness>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                            |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`         | :ref:`get_jiggle_joint_use_gravity<class_SkeletonModification2DJiggle_method_get_jiggle_joint_use_gravity>`\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const|                                        |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`         | :ref:`get_use_colliders<class_SkeletonModification2DJiggle_method_get_use_colliders>`\ (\ ) |const|                                                                                                 |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_collision_mask<class_SkeletonModification2DJiggle_method_set_collision_mask>`\ (\ collision_mask\: :ref:`int<class_int>`\ )                                                               |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_bone2d_node<class_SkeletonModification2DJiggle_method_set_jiggle_joint_bone2d_node>`\ (\ joint_idx\: :ref:`int<class_int>`, bone2d_node\: :ref:`NodePath<class_NodePath>`\ ) |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_bone_index<class_SkeletonModification2DJiggle_method_set_jiggle_joint_bone_index>`\ (\ joint_idx\: :ref:`int<class_int>`, bone_idx\: :ref:`int<class_int>`\ )                |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_damping<class_SkeletonModification2DJiggle_method_set_jiggle_joint_damping>`\ (\ joint_idx\: :ref:`int<class_int>`, damping\: :ref:`float<class_float>`\ )                   |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_gravity<class_SkeletonModification2DJiggle_method_set_jiggle_joint_gravity>`\ (\ joint_idx\: :ref:`int<class_int>`, gravity\: :ref:`Vector2<class_Vector2>`\ )               |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_mass<class_SkeletonModification2DJiggle_method_set_jiggle_joint_mass>`\ (\ joint_idx\: :ref:`int<class_int>`, mass\: :ref:`float<class_float>`\ )                            |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_override<class_SkeletonModification2DJiggle_method_set_jiggle_joint_override>`\ (\ joint_idx\: :ref:`int<class_int>`, override\: :ref:`bool<class_bool>`\ )                  |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_stiffness<class_SkeletonModification2DJiggle_method_set_jiggle_joint_stiffness>`\ (\ joint_idx\: :ref:`int<class_int>`, stiffness\: :ref:`float<class_float>`\ )             |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_jiggle_joint_use_gravity<class_SkeletonModification2DJiggle_method_set_jiggle_joint_use_gravity>`\ (\ joint_idx\: :ref:`int<class_int>`, use_gravity\: :ref:`bool<class_bool>`\ )         |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                          | :ref:`set_use_colliders<class_SkeletonModification2DJiggle_method_set_use_colliders>`\ (\ use_colliders\: :ref:`bool<class_bool>`\ )                                                                |
   +---------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_SkeletonModification2DJiggle_property_damping:

.. rst-class:: classref-property

:ref:`float<class_float>` **damping** = ``0.75`` :ref:`🔗<class_SkeletonModification2DJiggle_property_damping>`

.. rst-class:: classref-property-setget

- |void| **set_damping**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_damping**\ (\ )

The default amount of damping applied to the Jiggle joints, if they are not overridden. Higher values lead to more of the calculated velocity being applied.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_property_gravity:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **gravity** = ``Vector2(0, 6)`` :ref:`🔗<class_SkeletonModification2DJiggle_property_gravity>`

.. rst-class:: classref-property-setget

- |void| **set_gravity**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_gravity**\ (\ )

The default amount of gravity applied to the Jiggle joints, if they are not overridden.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_property_jiggle_data_chain_length:

.. rst-class:: classref-property

:ref:`int<class_int>` **jiggle_data_chain_length** = ``0`` :ref:`🔗<class_SkeletonModification2DJiggle_property_jiggle_data_chain_length>`

.. rst-class:: classref-property-setget

- |void| **set_jiggle_data_chain_length**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_jiggle_data_chain_length**\ (\ )

The amount of Jiggle joints in the Jiggle modification.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_property_mass:

.. rst-class:: classref-property

:ref:`float<class_float>` **mass** = ``0.75`` :ref:`🔗<class_SkeletonModification2DJiggle_property_mass>`

.. rst-class:: classref-property-setget

- |void| **set_mass**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_mass**\ (\ )

The default amount of mass assigned to the Jiggle joints, if they are not overridden. Higher values lead to faster movements and more overshooting.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_property_stiffness:

.. rst-class:: classref-property

:ref:`float<class_float>` **stiffness** = ``3.0`` :ref:`🔗<class_SkeletonModification2DJiggle_property_stiffness>`

.. rst-class:: classref-property-setget

- |void| **set_stiffness**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_stiffness**\ (\ )

The default amount of stiffness assigned to the Jiggle joints, if they are not overridden. Higher values act more like springs, quickly moving into the correct position.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_property_target_nodepath:

.. rst-class:: classref-property

:ref:`NodePath<class_NodePath>` **target_nodepath** = ``NodePath("")`` :ref:`🔗<class_SkeletonModification2DJiggle_property_target_nodepath>`

.. rst-class:: classref-property-setget

- |void| **set_target_node**\ (\ value\: :ref:`NodePath<class_NodePath>`\ )
- :ref:`NodePath<class_NodePath>` **get_target_node**\ (\ )

The NodePath to the node that is the target for the Jiggle modification. This node is what the Jiggle chain will attempt to rotate the bone chain to.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_property_use_gravity:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **use_gravity** = ``false`` :ref:`🔗<class_SkeletonModification2DJiggle_property_use_gravity>`

.. rst-class:: classref-property-setget

- |void| **set_use_gravity**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **get_use_gravity**\ (\ )

Whether the gravity vector, :ref:`gravity<class_SkeletonModification2DJiggle_property_gravity>`, should be applied to the Jiggle joints, assuming they are not overriding the default settings.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_SkeletonModification2DJiggle_method_get_collision_mask:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_collision_mask**\ (\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_collision_mask>`

Returns the collision mask used by the Jiggle modifier when collisions are enabled.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_bone2d_node:

.. rst-class:: classref-method

:ref:`NodePath<class_NodePath>` **get_jiggle_joint_bone2d_node**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_bone2d_node>`

Returns the :ref:`Bone2D<class_Bone2D>` node assigned to the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_bone_index:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_jiggle_joint_bone_index**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_bone_index>`

Returns the index of the :ref:`Bone2D<class_Bone2D>` node assigned to the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_damping:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_jiggle_joint_damping**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_damping>`

Returns the amount of damping of the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_gravity:

.. rst-class:: classref-method

:ref:`Vector2<class_Vector2>` **get_jiggle_joint_gravity**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_gravity>`

Returns a :ref:`Vector2<class_Vector2>` representing the amount of gravity the Jiggle joint at ``joint_idx`` is influenced by.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_mass:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_jiggle_joint_mass**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_mass>`

Returns the amount of mass of the jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_override:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **get_jiggle_joint_override**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_override>`

Returns a boolean that indicates whether the joint at ``joint_idx`` is overriding the default Jiggle joint data defined in the modification.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_stiffness:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_jiggle_joint_stiffness**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_stiffness>`

Returns the stiffness of the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_jiggle_joint_use_gravity:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **get_jiggle_joint_use_gravity**\ (\ joint_idx\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_jiggle_joint_use_gravity>`

Returns a boolean that indicates whether the joint at ``joint_idx`` is using gravity or not.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_get_use_colliders:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **get_use_colliders**\ (\ ) |const| :ref:`🔗<class_SkeletonModification2DJiggle_method_get_use_colliders>`

Returns whether the jiggle modifier is taking physics colliders into account when solving.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_collision_mask:

.. rst-class:: classref-method

|void| **set_collision_mask**\ (\ collision_mask\: :ref:`int<class_int>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_collision_mask>`

Sets the collision mask that the Jiggle modifier will use when reacting to colliders, if the Jiggle modifier is set to take colliders into account.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_bone2d_node:

.. rst-class:: classref-method

|void| **set_jiggle_joint_bone2d_node**\ (\ joint_idx\: :ref:`int<class_int>`, bone2d_node\: :ref:`NodePath<class_NodePath>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_bone2d_node>`

Sets the :ref:`Bone2D<class_Bone2D>` node assigned to the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_bone_index:

.. rst-class:: classref-method

|void| **set_jiggle_joint_bone_index**\ (\ joint_idx\: :ref:`int<class_int>`, bone_idx\: :ref:`int<class_int>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_bone_index>`

Sets the bone index, ``bone_idx``, of the Jiggle joint at ``joint_idx``. When possible, this will also update the ``bone2d_node`` of the Jiggle joint based on data provided by the linked skeleton.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_damping:

.. rst-class:: classref-method

|void| **set_jiggle_joint_damping**\ (\ joint_idx\: :ref:`int<class_int>`, damping\: :ref:`float<class_float>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_damping>`

Sets the amount of damping of the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_gravity:

.. rst-class:: classref-method

|void| **set_jiggle_joint_gravity**\ (\ joint_idx\: :ref:`int<class_int>`, gravity\: :ref:`Vector2<class_Vector2>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_gravity>`

Sets the gravity vector of the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_mass:

.. rst-class:: classref-method

|void| **set_jiggle_joint_mass**\ (\ joint_idx\: :ref:`int<class_int>`, mass\: :ref:`float<class_float>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_mass>`

Sets the of mass of the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_override:

.. rst-class:: classref-method

|void| **set_jiggle_joint_override**\ (\ joint_idx\: :ref:`int<class_int>`, override\: :ref:`bool<class_bool>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_override>`

Sets whether the Jiggle joint at ``joint_idx`` should override the default Jiggle joint settings. Setting this to ``true`` will make the joint use its own settings rather than the default ones attached to the modification.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_stiffness:

.. rst-class:: classref-method

|void| **set_jiggle_joint_stiffness**\ (\ joint_idx\: :ref:`int<class_int>`, stiffness\: :ref:`float<class_float>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_stiffness>`

Sets the of stiffness of the Jiggle joint at ``joint_idx``.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_jiggle_joint_use_gravity:

.. rst-class:: classref-method

|void| **set_jiggle_joint_use_gravity**\ (\ joint_idx\: :ref:`int<class_int>`, use_gravity\: :ref:`bool<class_bool>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_jiggle_joint_use_gravity>`

Sets whether the Jiggle joint at ``joint_idx`` should use gravity.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModification2DJiggle_method_set_use_colliders:

.. rst-class:: classref-method

|void| **set_use_colliders**\ (\ use_colliders\: :ref:`bool<class_bool>`\ ) :ref:`🔗<class_SkeletonModification2DJiggle_method_set_use_colliders>`

If ``true``, the Jiggle modifier will take colliders into account, keeping them from entering into these collision objects.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
