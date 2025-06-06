:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisualShaderNodeVectorOp.xml.

.. _class_VisualShaderNodeVectorOp:

VisualShaderNodeVectorOp
========================

**Inherits:** :ref:`VisualShaderNodeVectorBase<class_VisualShaderNodeVectorBase>` **<** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A vector operator to be used within the visual shader graph.

.. rst-class:: classref-introduction-group

Description
-----------

A visual shader node for use of vector operators. Operates on vector ``a`` and vector ``b``.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------------------------------------+-------------------------------------------------------------------+-------+
   | :ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` | :ref:`operator<class_VisualShaderNodeVectorOp_property_operator>` | ``0`` |
   +---------------------------------------------------------+-------------------------------------------------------------------+-------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_VisualShaderNodeVectorOp_Operator:

.. rst-class:: classref-enumeration

enum **Operator**: :ref:`🔗<enum_VisualShaderNodeVectorOp_Operator>`

.. _class_VisualShaderNodeVectorOp_constant_OP_ADD:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_ADD** = ``0``

Adds two vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_SUB:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_SUB** = ``1``

Subtracts a vector from a vector.

.. _class_VisualShaderNodeVectorOp_constant_OP_MUL:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_MUL** = ``2``

Multiplies two vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_DIV:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_DIV** = ``3``

Divides vector by vector.

.. _class_VisualShaderNodeVectorOp_constant_OP_MOD:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_MOD** = ``4``

Returns the remainder of the two vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_POW:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_POW** = ``5``

Returns the value of the first parameter raised to the power of the second, for each component of the vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_MAX** = ``6``

Returns the greater of two values, for each component of the vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_MIN:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_MIN** = ``7``

Returns the lesser of two values, for each component of the vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_CROSS:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_CROSS** = ``8``

Calculates the cross product of two vectors.

.. _class_VisualShaderNodeVectorOp_constant_OP_ATAN2:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_ATAN2** = ``9``

Returns the arc-tangent of the parameters.

.. _class_VisualShaderNodeVectorOp_constant_OP_REFLECT:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_REFLECT** = ``10``

Returns the vector that points in the direction of reflection. ``a`` is incident vector and ``b`` is the normal vector.

.. _class_VisualShaderNodeVectorOp_constant_OP_STEP:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_STEP** = ``11``

Vector step operator. Returns ``0.0`` if ``a`` is smaller than ``b`` and ``1.0`` otherwise.

.. _class_VisualShaderNodeVectorOp_constant_OP_ENUM_SIZE:

.. rst-class:: classref-enumeration-constant

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **OP_ENUM_SIZE** = ``12``

Represents the size of the :ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` enum.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisualShaderNodeVectorOp_property_operator:

.. rst-class:: classref-property

:ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **operator** = ``0`` :ref:`🔗<class_VisualShaderNodeVectorOp_property_operator>`

.. rst-class:: classref-property-setget

- |void| **set_operator**\ (\ value\: :ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>`\ )
- :ref:`Operator<enum_VisualShaderNodeVectorOp_Operator>` **get_operator**\ (\ )

The operator to be used.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
