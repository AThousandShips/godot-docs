:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/modules/csg/doc_classes/CSGCylinder3D.xml.

.. _class_CSGCylinder3D:

CSGCylinder3D
=============

**Inherits:** :ref:`CSGPrimitive3D<class_CSGPrimitive3D>` **<** :ref:`CSGShape3D<class_CSGShape3D>` **<** :ref:`GeometryInstance3D<class_GeometryInstance3D>` **<** :ref:`VisualInstance3D<class_VisualInstance3D>` **<** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A CSG Cylinder shape.

.. rst-class:: classref-introduction-group

Description
-----------

This node allows you to create a cylinder (or cone) for use with the CSG system.

\ **Note:** CSG nodes are intended to be used for level prototyping. Creating CSG nodes has a significant CPU cost compared to creating a :ref:`MeshInstance3D<class_MeshInstance3D>` with a :ref:`PrimitiveMesh<class_PrimitiveMesh>`. Moving a CSG node within another CSG node also has a significant CPU cost, so it should be avoided during gameplay.

.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`Prototyping levels with CSG <../tutorials/3d/csg_tools>`

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------------+----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`         | :ref:`cone<class_CSGCylinder3D_property_cone>`                 | ``false`` |
   +---------------------------------+----------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`       | :ref:`height<class_CSGCylinder3D_property_height>`             | ``2.0``   |
   +---------------------------------+----------------------------------------------------------------+-----------+
   | :ref:`Material<class_Material>` | :ref:`material<class_CSGCylinder3D_property_material>`         |           |
   +---------------------------------+----------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`       | :ref:`radius<class_CSGCylinder3D_property_radius>`             | ``0.5``   |
   +---------------------------------+----------------------------------------------------------------+-----------+
   | :ref:`int<class_int>`           | :ref:`sides<class_CSGCylinder3D_property_sides>`               | ``8``     |
   +---------------------------------+----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`         | :ref:`smooth_faces<class_CSGCylinder3D_property_smooth_faces>` | ``true``  |
   +---------------------------------+----------------------------------------------------------------+-----------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_CSGCylinder3D_property_cone:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **cone** = ``false`` :ref:`🔗<class_CSGCylinder3D_property_cone>`

.. rst-class:: classref-property-setget

- |void| **set_cone**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_cone**\ (\ )

If ``true`` a cone is created, the :ref:`radius<class_CSGCylinder3D_property_radius>` will only apply to one side.

.. rst-class:: classref-item-separator

----

.. _class_CSGCylinder3D_property_height:

.. rst-class:: classref-property

:ref:`float<class_float>` **height** = ``2.0`` :ref:`🔗<class_CSGCylinder3D_property_height>`

.. rst-class:: classref-property-setget

- |void| **set_height**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_height**\ (\ )

The height of the cylinder.

.. rst-class:: classref-item-separator

----

.. _class_CSGCylinder3D_property_material:

.. rst-class:: classref-property

:ref:`Material<class_Material>` **material** :ref:`🔗<class_CSGCylinder3D_property_material>`

.. rst-class:: classref-property-setget

- |void| **set_material**\ (\ value\: :ref:`Material<class_Material>`\ )
- :ref:`Material<class_Material>` **get_material**\ (\ )

The material used to render the cylinder.

.. rst-class:: classref-item-separator

----

.. _class_CSGCylinder3D_property_radius:

.. rst-class:: classref-property

:ref:`float<class_float>` **radius** = ``0.5`` :ref:`🔗<class_CSGCylinder3D_property_radius>`

.. rst-class:: classref-property-setget

- |void| **set_radius**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_radius**\ (\ )

The radius of the cylinder.

.. rst-class:: classref-item-separator

----

.. _class_CSGCylinder3D_property_sides:

.. rst-class:: classref-property

:ref:`int<class_int>` **sides** = ``8`` :ref:`🔗<class_CSGCylinder3D_property_sides>`

.. rst-class:: classref-property-setget

- |void| **set_sides**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_sides**\ (\ )

The number of sides of the cylinder, the higher this number the more detail there will be in the cylinder.

.. rst-class:: classref-item-separator

----

.. _class_CSGCylinder3D_property_smooth_faces:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **smooth_faces** = ``true`` :ref:`🔗<class_CSGCylinder3D_property_smooth_faces>`

.. rst-class:: classref-property-setget

- |void| **set_smooth_faces**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **get_smooth_faces**\ (\ )

If ``true`` the normals of the cylinder are set to give a smooth effect making the cylinder seem rounded. If ``false`` the cylinder will have a flat shaded look.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
