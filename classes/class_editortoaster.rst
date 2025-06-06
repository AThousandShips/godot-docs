:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/EditorToaster.xml.

.. _class_EditorToaster:

EditorToaster
=============

**Inherits:** :ref:`HBoxContainer<class_HBoxContainer>` **<** :ref:`BoxContainer<class_BoxContainer>` **<** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Manages toast notifications within the editor.

.. rst-class:: classref-introduction-group

Description
-----------

This object manages the functionality and display of toast notifications within the editor, ensuring timely and informative alerts are presented to users.

\ **Note:** This class shouldn't be instantiated directly. Instead, access the singleton using :ref:`EditorInterface.get_editor_toaster()<class_EditorInterface_method_get_editor_toaster>`.

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +--------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void| | :ref:`push_toast<class_EditorToaster_method_push_toast>`\ (\ message\: :ref:`String<class_String>`, severity\: :ref:`Severity<enum_EditorToaster_Severity>` = 0, tooltip\: :ref:`String<class_String>` = ""\ ) |
   +--------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_EditorToaster_Severity:

.. rst-class:: classref-enumeration

enum **Severity**: :ref:`🔗<enum_EditorToaster_Severity>`

.. _class_EditorToaster_constant_SEVERITY_INFO:

.. rst-class:: classref-enumeration-constant

:ref:`Severity<enum_EditorToaster_Severity>` **SEVERITY_INFO** = ``0``

Toast will display with an INFO severity.

.. _class_EditorToaster_constant_SEVERITY_WARNING:

.. rst-class:: classref-enumeration-constant

:ref:`Severity<enum_EditorToaster_Severity>` **SEVERITY_WARNING** = ``1``

Toast will display with a WARNING severity and have a corresponding color.

.. _class_EditorToaster_constant_SEVERITY_ERROR:

.. rst-class:: classref-enumeration-constant

:ref:`Severity<enum_EditorToaster_Severity>` **SEVERITY_ERROR** = ``2``

Toast will display with an ERROR severity and have a corresponding color.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_EditorToaster_method_push_toast:

.. rst-class:: classref-method

|void| **push_toast**\ (\ message\: :ref:`String<class_String>`, severity\: :ref:`Severity<enum_EditorToaster_Severity>` = 0, tooltip\: :ref:`String<class_String>` = ""\ ) :ref:`🔗<class_EditorToaster_method_push_toast>`

Pushes a toast notification to the editor for display.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
