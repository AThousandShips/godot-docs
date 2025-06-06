:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisualShaderNodeTexture.xml.

.. _class_VisualShaderNodeTexture:

VisualShaderNodeTexture
=======================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Performs a 2D texture lookup within the visual shader graph.

.. rst-class:: classref-introduction-group

Description
-----------

Performs a lookup operation on the provided texture, with support for multiple texture sources to choose from.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +--------------------------------------------------------------+--------------------------------------------------------------------------+-------+
   | :ref:`Source<enum_VisualShaderNodeTexture_Source>`           | :ref:`source<class_VisualShaderNodeTexture_property_source>`             | ``0`` |
   +--------------------------------------------------------------+--------------------------------------------------------------------------+-------+
   | :ref:`Texture2D<class_Texture2D>`                            | :ref:`texture<class_VisualShaderNodeTexture_property_texture>`           |       |
   +--------------------------------------------------------------+--------------------------------------------------------------------------+-------+
   | :ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` | :ref:`texture_type<class_VisualShaderNodeTexture_property_texture_type>` | ``0`` |
   +--------------------------------------------------------------+--------------------------------------------------------------------------+-------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_VisualShaderNodeTexture_Source:

.. rst-class:: classref-enumeration

enum **Source**: :ref:`🔗<enum_VisualShaderNodeTexture_Source>`

.. _class_VisualShaderNodeTexture_constant_SOURCE_TEXTURE:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_TEXTURE** = ``0``

Use the texture given as an argument for this function.

.. _class_VisualShaderNodeTexture_constant_SOURCE_SCREEN:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_SCREEN** = ``1``

Use the current viewport's texture as the source.

.. _class_VisualShaderNodeTexture_constant_SOURCE_2D_TEXTURE:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_2D_TEXTURE** = ``2``

Use the texture from this shader's texture built-in (e.g. a texture of a :ref:`Sprite2D<class_Sprite2D>`).

.. _class_VisualShaderNodeTexture_constant_SOURCE_2D_NORMAL:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_2D_NORMAL** = ``3``

Use the texture from this shader's normal map built-in.

.. _class_VisualShaderNodeTexture_constant_SOURCE_DEPTH:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_DEPTH** = ``4``

Use the depth texture captured during the depth prepass. Only available when the depth prepass is used (i.e. in spatial shaders and in the forward_plus or gl_compatibility renderers).

.. _class_VisualShaderNodeTexture_constant_SOURCE_PORT:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_PORT** = ``5``

Use the texture provided in the input port for this function.

.. _class_VisualShaderNodeTexture_constant_SOURCE_3D_NORMAL:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_3D_NORMAL** = ``6``

Use the normal buffer captured during the depth prepass. Only available when the normal-roughness buffer is available (i.e. in spatial shaders and in the forward_plus renderer).

.. _class_VisualShaderNodeTexture_constant_SOURCE_ROUGHNESS:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_ROUGHNESS** = ``7``

Use the roughness buffer captured during the depth prepass. Only available when the normal-roughness buffer is available (i.e. in spatial shaders and in the forward_plus renderer).

.. _class_VisualShaderNodeTexture_constant_SOURCE_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **SOURCE_MAX** = ``8``

Represents the size of the :ref:`Source<enum_VisualShaderNodeTexture_Source>` enum.

.. rst-class:: classref-item-separator

----

.. _enum_VisualShaderNodeTexture_TextureType:

.. rst-class:: classref-enumeration

enum **TextureType**: :ref:`🔗<enum_VisualShaderNodeTexture_TextureType>`

.. _class_VisualShaderNodeTexture_constant_TYPE_DATA:

.. rst-class:: classref-enumeration-constant

:ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` **TYPE_DATA** = ``0``

No hints are added to the uniform declaration.

.. _class_VisualShaderNodeTexture_constant_TYPE_COLOR:

.. rst-class:: classref-enumeration-constant

:ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` **TYPE_COLOR** = ``1``

Adds ``source_color`` as hint to the uniform declaration for proper sRGB to linear conversion.

.. _class_VisualShaderNodeTexture_constant_TYPE_NORMAL_MAP:

.. rst-class:: classref-enumeration-constant

:ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` **TYPE_NORMAL_MAP** = ``2``

Adds ``hint_normal`` as hint to the uniform declaration, which internally converts the texture for proper usage as normal map.

.. _class_VisualShaderNodeTexture_constant_TYPE_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` **TYPE_MAX** = ``3``

Represents the size of the :ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` enum.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisualShaderNodeTexture_property_source:

.. rst-class:: classref-property

:ref:`Source<enum_VisualShaderNodeTexture_Source>` **source** = ``0`` :ref:`🔗<class_VisualShaderNodeTexture_property_source>`

.. rst-class:: classref-property-setget

- |void| **set_source**\ (\ value\: :ref:`Source<enum_VisualShaderNodeTexture_Source>`\ )
- :ref:`Source<enum_VisualShaderNodeTexture_Source>` **get_source**\ (\ )

Determines the source for the lookup.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeTexture_property_texture:

.. rst-class:: classref-property

:ref:`Texture2D<class_Texture2D>` **texture** :ref:`🔗<class_VisualShaderNodeTexture_property_texture>`

.. rst-class:: classref-property-setget

- |void| **set_texture**\ (\ value\: :ref:`Texture2D<class_Texture2D>`\ )
- :ref:`Texture2D<class_Texture2D>` **get_texture**\ (\ )

The source texture, if needed for the selected :ref:`source<class_VisualShaderNodeTexture_property_source>`.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeTexture_property_texture_type:

.. rst-class:: classref-property

:ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` **texture_type** = ``0`` :ref:`🔗<class_VisualShaderNodeTexture_property_texture_type>`

.. rst-class:: classref-property-setget

- |void| **set_texture_type**\ (\ value\: :ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>`\ )
- :ref:`TextureType<enum_VisualShaderNodeTexture_TextureType>` **get_texture_type**\ (\ )

Specifies the type of the texture if :ref:`source<class_VisualShaderNodeTexture_property_source>` is set to :ref:`SOURCE_TEXTURE<class_VisualShaderNodeTexture_constant_SOURCE_TEXTURE>`.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
