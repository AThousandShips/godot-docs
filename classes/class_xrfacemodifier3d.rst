:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/XRFaceModifier3D.xml.

.. _class_XRFaceModifier3D:

XRFaceModifier3D
================

**Experimental:** This class may be changed or removed in future versions.

**Inherits:** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A node for driving standard face meshes from :ref:`XRFaceTracker<class_XRFaceTracker>` weights.

.. rst-class:: classref-introduction-group

Description
-----------

This node applies weights from an :ref:`XRFaceTracker<class_XRFaceTracker>` to a mesh with supporting face blend shapes.

The `Unified Expressions <https://docs.vrcft.io/docs/tutorial-avatars/tutorial-avatars-extras/unified-blendshapes>`__ blend shapes are supported, as well as ARKit and SRanipal blend shapes.

The node attempts to identify blend shapes based on name matching. Blend shapes should match the names listed in the `Unified Expressions Compatibility <https://docs.vrcft.io/docs/tutorial-avatars/tutorial-avatars-extras/compatibility/overview>`__ chart.

.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`XR documentation index <../tutorials/xr/index>`

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------------+-------------------------------------------------------------------+---------------------------+
   | :ref:`StringName<class_StringName>` | :ref:`face_tracker<class_XRFaceModifier3D_property_face_tracker>` | ``&"/user/face_tracker"`` |
   +-------------------------------------+-------------------------------------------------------------------+---------------------------+
   | :ref:`NodePath<class_NodePath>`     | :ref:`target<class_XRFaceModifier3D_property_target>`             | ``NodePath("")``          |
   +-------------------------------------+-------------------------------------------------------------------+---------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_XRFaceModifier3D_property_face_tracker:

.. rst-class:: classref-property

:ref:`StringName<class_StringName>` **face_tracker** = ``&"/user/face_tracker"`` :ref:`🔗<class_XRFaceModifier3D_property_face_tracker>`

.. rst-class:: classref-property-setget

- |void| **set_face_tracker**\ (\ value\: :ref:`StringName<class_StringName>`\ )
- :ref:`StringName<class_StringName>` **get_face_tracker**\ (\ )

The :ref:`XRFaceTracker<class_XRFaceTracker>` path.

.. rst-class:: classref-item-separator

----

.. _class_XRFaceModifier3D_property_target:

.. rst-class:: classref-property

:ref:`NodePath<class_NodePath>` **target** = ``NodePath("")`` :ref:`🔗<class_XRFaceModifier3D_property_target>`

.. rst-class:: classref-property-setget

- |void| **set_target**\ (\ value\: :ref:`NodePath<class_NodePath>`\ )
- :ref:`NodePath<class_NodePath>` **get_target**\ (\ )

The :ref:`NodePath<class_NodePath>` of the face :ref:`MeshInstance3D<class_MeshInstance3D>`.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
