:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/PortableCompressedTexture2D.xml.

.. _class_PortableCompressedTexture2D:

PortableCompressedTexture2D
===========================

**Inherits:** :ref:`Texture2D<class_Texture2D>` **<** :ref:`Texture<class_Texture>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Provides a compressed texture for disk and/or VRAM in a way that is portable.

.. rst-class:: classref-introduction-group

Description
-----------

This class allows storing compressed textures as self contained (not imported) resources.

For 2D usage (compressed on disk, uncompressed on VRAM), the lossy and lossless modes are recommended. For 3D usage (compressed on VRAM) it depends on the target platform.

If you intend to only use desktop, S3TC or BPTC are recommended. For only mobile, ETC2 is recommended.

For portable, self contained 3D textures that work on both desktop and mobile, Basis Universal is recommended (although it has a small quality cost and longer compression time as a tradeoff).

This resource is intended to be created from code.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------+--------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`       | :ref:`keep_compressed_buffer<class_PortableCompressedTexture2D_property_keep_compressed_buffer>` | ``false``                                                                              |
   +-------------------------------+--------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`       | resource_local_to_scene                                                                          | ``false`` (overrides :ref:`Resource<class_Resource_property_resource_local_to_scene>`) |
   +-------------------------------+--------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`size_override<class_PortableCompressedTexture2D_property_size_override>`                   | ``Vector2(0, 0)``                                                                      |
   +-------------------------------+--------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                                   | :ref:`create_from_image<class_PortableCompressedTexture2D_method_create_from_image>`\ (\ image\: :ref:`Image<class_Image>`, compression_mode\: :ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>`, normal_map\: :ref:`bool<class_bool>` = false, lossy_quality\: :ref:`float<class_float>` = 0.8\ ) |
   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` | :ref:`get_compression_mode<class_PortableCompressedTexture2D_method_get_compression_mode>`\ (\ ) |const|                                                                                                                                                                                                                  |
   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Format<enum_Image_Format>`                                         | :ref:`get_format<class_PortableCompressedTexture2D_method_get_format>`\ (\ ) |const|                                                                                                                                                                                                                                      |
   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                                                  | :ref:`is_keeping_all_compressed_buffers<class_PortableCompressedTexture2D_method_is_keeping_all_compressed_buffers>`\ (\ ) |static|                                                                                                                                                                                       |
   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                                   | :ref:`set_basisu_compressor_params<class_PortableCompressedTexture2D_method_set_basisu_compressor_params>`\ (\ uastc_level\: :ref:`int<class_int>`, rdo_quality_loss\: :ref:`float<class_float>`\ )                                                                                                                       |
   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                                   | :ref:`set_keep_all_compressed_buffers<class_PortableCompressedTexture2D_method_set_keep_all_compressed_buffers>`\ (\ keep\: :ref:`bool<class_bool>`\ ) |static|                                                                                                                                                           |
   +--------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_PortableCompressedTexture2D_CompressionMode:

.. rst-class:: classref-enumeration

enum **CompressionMode**: :ref:`🔗<enum_PortableCompressedTexture2D_CompressionMode>`

.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_LOSSLESS:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_LOSSLESS** = ``0``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_LOSSY:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_LOSSY** = ``1``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_BASIS_UNIVERSAL:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_BASIS_UNIVERSAL** = ``2``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_S3TC:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_S3TC** = ``3``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_ETC2:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_ETC2** = ``4``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_BPTC:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_BPTC** = ``5``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. _class_PortableCompressedTexture2D_constant_COMPRESSION_MODE_ASTC:

.. rst-class:: classref-enumeration-constant

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **COMPRESSION_MODE_ASTC** = ``6``

.. container:: contribute

	There is currently no description for this enum. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!



.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_PortableCompressedTexture2D_property_keep_compressed_buffer:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **keep_compressed_buffer** = ``false`` :ref:`🔗<class_PortableCompressedTexture2D_property_keep_compressed_buffer>`

.. rst-class:: classref-property-setget

- |void| **set_keep_compressed_buffer**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_keeping_compressed_buffer**\ (\ )

When running on the editor, this class will keep the source compressed data in memory. Otherwise, the source compressed data is lost after loading and the resource can't be re saved.

This flag allows to keep the compressed data in memory if you intend it to persist after loading.

\ **Note:** This must be set before :ref:`create_from_image()<class_PortableCompressedTexture2D_method_create_from_image>` to take effect.

.. rst-class:: classref-item-separator

----

.. _class_PortableCompressedTexture2D_property_size_override:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **size_override** = ``Vector2(0, 0)`` :ref:`🔗<class_PortableCompressedTexture2D_property_size_override>`

.. rst-class:: classref-property-setget

- |void| **set_size_override**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_size_override**\ (\ )

Allow overriding the texture size (for 2D only).

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_PortableCompressedTexture2D_method_create_from_image:

.. rst-class:: classref-method

|void| **create_from_image**\ (\ image\: :ref:`Image<class_Image>`, compression_mode\: :ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>`, normal_map\: :ref:`bool<class_bool>` = false, lossy_quality\: :ref:`float<class_float>` = 0.8\ ) :ref:`🔗<class_PortableCompressedTexture2D_method_create_from_image>`

Initializes the compressed texture from a base image. The compression mode must be provided.

\ ``normal_map`` is recommended to ensure optimum quality if this image will be used as a normal map.

If lossy compression is requested, the quality setting can optionally be provided. This maps to Lossy WebP compression quality.

.. rst-class:: classref-item-separator

----

.. _class_PortableCompressedTexture2D_method_get_compression_mode:

.. rst-class:: classref-method

:ref:`CompressionMode<enum_PortableCompressedTexture2D_CompressionMode>` **get_compression_mode**\ (\ ) |const| :ref:`🔗<class_PortableCompressedTexture2D_method_get_compression_mode>`

Return the compression mode used (valid after initialized).

.. rst-class:: classref-item-separator

----

.. _class_PortableCompressedTexture2D_method_get_format:

.. rst-class:: classref-method

:ref:`Format<enum_Image_Format>` **get_format**\ (\ ) |const| :ref:`🔗<class_PortableCompressedTexture2D_method_get_format>`

Return the image format used (valid after initialized).

.. rst-class:: classref-item-separator

----

.. _class_PortableCompressedTexture2D_method_is_keeping_all_compressed_buffers:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_keeping_all_compressed_buffers**\ (\ ) |static| :ref:`🔗<class_PortableCompressedTexture2D_method_is_keeping_all_compressed_buffers>`

Return whether the flag is overridden for all textures of this type.

.. rst-class:: classref-item-separator

----

.. _class_PortableCompressedTexture2D_method_set_basisu_compressor_params:

.. rst-class:: classref-method

|void| **set_basisu_compressor_params**\ (\ uastc_level\: :ref:`int<class_int>`, rdo_quality_loss\: :ref:`float<class_float>`\ ) :ref:`🔗<class_PortableCompressedTexture2D_method_set_basisu_compressor_params>`

Sets the compressor parameters for Basis Universal compression. See also the settings in :ref:`ResourceImporterTexture<class_ResourceImporterTexture>`.

\ **Note:** This must be set before :ref:`create_from_image()<class_PortableCompressedTexture2D_method_create_from_image>` to take effect.

.. rst-class:: classref-item-separator

----

.. _class_PortableCompressedTexture2D_method_set_keep_all_compressed_buffers:

.. rst-class:: classref-method

|void| **set_keep_all_compressed_buffers**\ (\ keep\: :ref:`bool<class_bool>`\ ) |static| :ref:`🔗<class_PortableCompressedTexture2D_method_set_keep_all_compressed_buffers>`

Overrides the flag globally for all textures of this type. This is used primarily by the editor.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
