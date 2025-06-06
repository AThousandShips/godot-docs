:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/EditorFileSystemImportFormatSupportQuery.xml.

.. _class_EditorFileSystemImportFormatSupportQuery:

EditorFileSystemImportFormatSupportQuery
========================================

**Inherits:** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Used to query and configure import format support.

.. rst-class:: classref-introduction-group

Description
-----------

This class is used to query and configure a certain import format. It is used in conjunction with asset format import plugins.

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>` | :ref:`_get_file_extensions<class_EditorFileSystemImportFormatSupportQuery_private_method__get_file_extensions>`\ (\ ) |virtual| |required| |const| |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                           | :ref:`_is_active<class_EditorFileSystemImportFormatSupportQuery_private_method__is_active>`\ (\ ) |virtual| |required| |const|                     |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                           | :ref:`_query<class_EditorFileSystemImportFormatSupportQuery_private_method__query>`\ (\ ) |virtual| |required| |const|                             |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_EditorFileSystemImportFormatSupportQuery_private_method__get_file_extensions:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **_get_file_extensions**\ (\ ) |virtual| |required| |const| :ref:`🔗<class_EditorFileSystemImportFormatSupportQuery_private_method__get_file_extensions>`

Return the file extensions supported.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileSystemImportFormatSupportQuery_private_method__is_active:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **_is_active**\ (\ ) |virtual| |required| |const| :ref:`🔗<class_EditorFileSystemImportFormatSupportQuery_private_method__is_active>`

Return whether this importer is active.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileSystemImportFormatSupportQuery_private_method__query:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **_query**\ (\ ) |virtual| |required| |const| :ref:`🔗<class_EditorFileSystemImportFormatSupportQuery_private_method__query>`

Query support. Return ``false`` if import must not continue.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
