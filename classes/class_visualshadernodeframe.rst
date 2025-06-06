:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisualShaderNodeFrame.xml.

.. _class_VisualShaderNodeFrame:

VisualShaderNodeFrame
=====================

**Inherits:** :ref:`VisualShaderNodeResizableBase<class_VisualShaderNodeResizableBase>` **<** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`VisualShaderNodeComment<class_VisualShaderNodeComment>`

A frame other visual shader nodes can be attached to for better organization.

.. rst-class:: classref-introduction-group

Description
-----------

A rectangular frame that can be used to group visual shader nodes together to improve organization.

Nodes attached to the frame will move with it when it is dragged and it can automatically resize to enclose all attached nodes.

Its title, description and color can be customized.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------+
   | :ref:`PackedInt32Array<class_PackedInt32Array>` | :ref:`attached_nodes<class_VisualShaderNodeFrame_property_attached_nodes>`         | ``PackedInt32Array()``         |
   +-------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`autoshrink<class_VisualShaderNodeFrame_property_autoshrink>`                 | ``true``                       |
   +-------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------+
   | :ref:`Color<class_Color>`                       | :ref:`tint_color<class_VisualShaderNodeFrame_property_tint_color>`                 | ``Color(0.3, 0.3, 0.3, 0.75)`` |
   +-------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`tint_color_enabled<class_VisualShaderNodeFrame_property_tint_color_enabled>` | ``false``                      |
   +-------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------+
   | :ref:`String<class_String>`                     | :ref:`title<class_VisualShaderNodeFrame_property_title>`                           | ``"Title"``                    |
   +-------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +--------+--------------------------------------------------------------------------------------------------------------------------+
   | |void| | :ref:`add_attached_node<class_VisualShaderNodeFrame_method_add_attached_node>`\ (\ node\: :ref:`int<class_int>`\ )       |
   +--------+--------------------------------------------------------------------------------------------------------------------------+
   | |void| | :ref:`remove_attached_node<class_VisualShaderNodeFrame_method_remove_attached_node>`\ (\ node\: :ref:`int<class_int>`\ ) |
   +--------+--------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisualShaderNodeFrame_property_attached_nodes:

.. rst-class:: classref-property

:ref:`PackedInt32Array<class_PackedInt32Array>` **attached_nodes** = ``PackedInt32Array()`` :ref:`🔗<class_VisualShaderNodeFrame_property_attached_nodes>`

.. rst-class:: classref-property-setget

- |void| **set_attached_nodes**\ (\ value\: :ref:`PackedInt32Array<class_PackedInt32Array>`\ )
- :ref:`PackedInt32Array<class_PackedInt32Array>` **get_attached_nodes**\ (\ )

The list of nodes attached to the frame.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedInt32Array<class_PackedInt32Array>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeFrame_property_autoshrink:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **autoshrink** = ``true`` :ref:`🔗<class_VisualShaderNodeFrame_property_autoshrink>`

.. rst-class:: classref-property-setget

- |void| **set_autoshrink_enabled**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_autoshrink_enabled**\ (\ )

If ``true``, the frame will automatically resize to enclose all attached nodes.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeFrame_property_tint_color:

.. rst-class:: classref-property

:ref:`Color<class_Color>` **tint_color** = ``Color(0.3, 0.3, 0.3, 0.75)`` :ref:`🔗<class_VisualShaderNodeFrame_property_tint_color>`

.. rst-class:: classref-property-setget

- |void| **set_tint_color**\ (\ value\: :ref:`Color<class_Color>`\ )
- :ref:`Color<class_Color>` **get_tint_color**\ (\ )

The color of the frame when :ref:`tint_color_enabled<class_VisualShaderNodeFrame_property_tint_color_enabled>` is ``true``.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeFrame_property_tint_color_enabled:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **tint_color_enabled** = ``false`` :ref:`🔗<class_VisualShaderNodeFrame_property_tint_color_enabled>`

.. rst-class:: classref-property-setget

- |void| **set_tint_color_enabled**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_tint_color_enabled**\ (\ )

If ``true``, the frame will be tinted with the color specified in :ref:`tint_color<class_VisualShaderNodeFrame_property_tint_color>`.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeFrame_property_title:

.. rst-class:: classref-property

:ref:`String<class_String>` **title** = ``"Title"`` :ref:`🔗<class_VisualShaderNodeFrame_property_title>`

.. rst-class:: classref-property-setget

- |void| **set_title**\ (\ value\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_title**\ (\ )

The title of the node.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_VisualShaderNodeFrame_method_add_attached_node:

.. rst-class:: classref-method

|void| **add_attached_node**\ (\ node\: :ref:`int<class_int>`\ ) :ref:`🔗<class_VisualShaderNodeFrame_method_add_attached_node>`

Adds a node to the list of nodes attached to the frame. Should not be called directly, use the :ref:`VisualShader.attach_node_to_frame()<class_VisualShader_method_attach_node_to_frame>` method instead.

.. rst-class:: classref-item-separator

----

.. _class_VisualShaderNodeFrame_method_remove_attached_node:

.. rst-class:: classref-method

|void| **remove_attached_node**\ (\ node\: :ref:`int<class_int>`\ ) :ref:`🔗<class_VisualShaderNodeFrame_method_remove_attached_node>`

Removes a node from the list of nodes attached to the frame. Should not be called directly, use the :ref:`VisualShader.detach_node_from_frame()<class_VisualShader_method_detach_node_from_frame>` method instead.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
