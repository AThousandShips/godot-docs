:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/CurveTexture.xml.

.. _class_CurveTexture:

CurveTexture
============

**Inherits:** :ref:`Texture2D<class_Texture2D>` **<** :ref:`Texture<class_Texture>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A 1D texture where pixel brightness corresponds to points on a curve.

.. rst-class:: classref-introduction-group

Description
-----------

A 1D texture where pixel brightness corresponds to points on a unit :ref:`Curve<class_Curve>` resource, either in grayscale or in red. This visual representation simplifies the task of saving curves as image files.

If you need to store up to 3 curves within a single texture, use :ref:`CurveXYZTexture<class_CurveXYZTexture>` instead. See also :ref:`GradientTexture1D<class_GradientTexture1D>` and :ref:`GradientTexture2D<class_GradientTexture2D>`.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------------------------------+---------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`Curve<class_Curve>`                         | :ref:`curve<class_CurveTexture_property_curve>`               |                                                                                        |
   +---------------------------------------------------+---------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                           | resource_local_to_scene                                       | ``false`` (overrides :ref:`Resource<class_Resource_property_resource_local_to_scene>`) |
   +---------------------------------------------------+---------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`TextureMode<enum_CurveTexture_TextureMode>` | :ref:`texture_mode<class_CurveTexture_property_texture_mode>` | ``0``                                                                                  |
   +---------------------------------------------------+---------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                             | :ref:`width<class_CurveTexture_property_width>`               | ``256``                                                                                |
   +---------------------------------------------------+---------------------------------------------------------------+----------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_CurveTexture_TextureMode:

.. rst-class:: classref-enumeration

enum **TextureMode**: :ref:`🔗<enum_CurveTexture_TextureMode>`

.. _class_CurveTexture_constant_TEXTURE_MODE_RGB:

.. rst-class:: classref-enumeration-constant

:ref:`TextureMode<enum_CurveTexture_TextureMode>` **TEXTURE_MODE_RGB** = ``0``

Store the curve equally across the red, green and blue channels. This uses more video memory, but is more compatible with shaders that only read the green and blue values.

.. _class_CurveTexture_constant_TEXTURE_MODE_RED:

.. rst-class:: classref-enumeration-constant

:ref:`TextureMode<enum_CurveTexture_TextureMode>` **TEXTURE_MODE_RED** = ``1``

Store the curve only in the red channel. This saves video memory, but some custom shaders may not be able to work with this.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_CurveTexture_property_curve:

.. rst-class:: classref-property

:ref:`Curve<class_Curve>` **curve** :ref:`🔗<class_CurveTexture_property_curve>`

.. rst-class:: classref-property-setget

- |void| **set_curve**\ (\ value\: :ref:`Curve<class_Curve>`\ )
- :ref:`Curve<class_Curve>` **get_curve**\ (\ )

The :ref:`Curve<class_Curve>` that is rendered onto the texture. Should be a unit :ref:`Curve<class_Curve>`.

.. rst-class:: classref-item-separator

----

.. _class_CurveTexture_property_texture_mode:

.. rst-class:: classref-property

:ref:`TextureMode<enum_CurveTexture_TextureMode>` **texture_mode** = ``0`` :ref:`🔗<class_CurveTexture_property_texture_mode>`

.. rst-class:: classref-property-setget

- |void| **set_texture_mode**\ (\ value\: :ref:`TextureMode<enum_CurveTexture_TextureMode>`\ )
- :ref:`TextureMode<enum_CurveTexture_TextureMode>` **get_texture_mode**\ (\ )

The format the texture should be generated with. When passing a CurveTexture as an input to a :ref:`Shader<class_Shader>`, this may need to be adjusted.

.. rst-class:: classref-item-separator

----

.. _class_CurveTexture_property_width:

.. rst-class:: classref-property

:ref:`int<class_int>` **width** = ``256`` :ref:`🔗<class_CurveTexture_property_width>`

.. rst-class:: classref-property-setget

- |void| **set_width**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_width**\ (\ )

The width of the texture (in pixels). Higher values make it possible to represent high-frequency data better (such as sudden direction changes), at the cost of increased generation time and memory usage.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
