:github_url: hide

.. meta::
	:keywords: batch

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/MultiMeshInstance2D.xml.

.. _class_MultiMeshInstance2D:

MultiMeshInstance2D
===================

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Node that instances a :ref:`MultiMesh<class_MultiMesh>` in 2D.

.. rst-class:: classref-introduction-group

Description
-----------

**MultiMeshInstance2D** is a specialized node to instance a :ref:`MultiMesh<class_MultiMesh>` resource in 2D.

Usage is the same as :ref:`MultiMeshInstance3D<class_MultiMeshInstance3D>`.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-----------------------------------+----------------------------------------------------------------+
   | :ref:`MultiMesh<class_MultiMesh>` | :ref:`multimesh<class_MultiMeshInstance2D_property_multimesh>` |
   +-----------------------------------+----------------------------------------------------------------+
   | :ref:`Texture2D<class_Texture2D>` | :ref:`texture<class_MultiMeshInstance2D_property_texture>`     |
   +-----------------------------------+----------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_MultiMeshInstance2D_signal_texture_changed:

.. rst-class:: classref-signal

**texture_changed**\ (\ ) :ref:`🔗<class_MultiMeshInstance2D_signal_texture_changed>`

Emitted when the :ref:`texture<class_MultiMeshInstance2D_property_texture>` is changed.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_MultiMeshInstance2D_property_multimesh:

.. rst-class:: classref-property

:ref:`MultiMesh<class_MultiMesh>` **multimesh** :ref:`🔗<class_MultiMeshInstance2D_property_multimesh>`

.. rst-class:: classref-property-setget

- |void| **set_multimesh**\ (\ value\: :ref:`MultiMesh<class_MultiMesh>`\ )
- :ref:`MultiMesh<class_MultiMesh>` **get_multimesh**\ (\ )

The :ref:`MultiMesh<class_MultiMesh>` that will be drawn by the **MultiMeshInstance2D**.

.. rst-class:: classref-item-separator

----

.. _class_MultiMeshInstance2D_property_texture:

.. rst-class:: classref-property

:ref:`Texture2D<class_Texture2D>` **texture** :ref:`🔗<class_MultiMeshInstance2D_property_texture>`

.. rst-class:: classref-property-setget

- |void| **set_texture**\ (\ value\: :ref:`Texture2D<class_Texture2D>`\ )
- :ref:`Texture2D<class_Texture2D>` **get_texture**\ (\ )

The :ref:`Texture2D<class_Texture2D>` that will be used if using the default :ref:`CanvasItemMaterial<class_CanvasItemMaterial>`. Can be accessed as ``TEXTURE`` in CanvasItem shader.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
