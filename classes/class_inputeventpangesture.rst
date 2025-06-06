:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/InputEventPanGesture.xml.

.. _class_InputEventPanGesture:

InputEventPanGesture
====================

**Inherits:** :ref:`InputEventGesture<class_InputEventGesture>` **<** :ref:`InputEventWithModifiers<class_InputEventWithModifiers>` **<** :ref:`InputEventFromWindow<class_InputEventFromWindow>` **<** :ref:`InputEvent<class_InputEvent>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Represents a panning touch gesture.

.. rst-class:: classref-introduction-group

Description
-----------

Stores information about pan gestures. A pan gesture is performed when the user swipes the touch screen with two fingers. It's typically used for panning/scrolling.

\ **Note:** On Android, this requires the :ref:`ProjectSettings.input_devices/pointing/android/enable_pan_and_scale_gestures<class_ProjectSettings_property_input_devices/pointing/android/enable_pan_and_scale_gestures>` project setting to be enabled.

.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`Using InputEvent <../tutorials/inputs/inputevent>`

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------+---------------------------------------------------------+-------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`delta<class_InputEventPanGesture_property_delta>` | ``Vector2(0, 0)`` |
   +-------------------------------+---------------------------------------------------------+-------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_InputEventPanGesture_property_delta:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **delta** = ``Vector2(0, 0)`` :ref:`🔗<class_InputEventPanGesture_property_delta>`

.. rst-class:: classref-property-setget

- |void| **set_delta**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_delta**\ (\ )

Panning amount since last pan event.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
