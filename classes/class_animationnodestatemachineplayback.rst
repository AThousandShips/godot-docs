:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/AnimationNodeStateMachinePlayback.xml.

.. _class_AnimationNodeStateMachinePlayback:

AnimationNodeStateMachinePlayback
=================================

**Inherits:** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Provides playback control for an :ref:`AnimationNodeStateMachine<class_AnimationNodeStateMachine>`.

.. rst-class:: classref-introduction-group

Description
-----------

Allows control of :ref:`AnimationTree<class_AnimationTree>` state machines created with :ref:`AnimationNodeStateMachine<class_AnimationNodeStateMachine>`. Retrieve with ``$AnimationTree.get("parameters/playback")``.


.. tabs::

 .. code-tab:: gdscript

    var state_machine = $AnimationTree.get("parameters/playback")
    state_machine.travel("some_state")

 .. code-tab:: csharp

    var stateMachine = GetNode<AnimationTree>("AnimationTree").Get("parameters/playback").As<AnimationNodeStateMachinePlayback>();
    stateMachine.Travel("some_state");



.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`Using AnimationTree <../tutorials/animation/animation_tree>`

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------+-------------------------+---------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>` | resource_local_to_scene | ``true`` (overrides :ref:`Resource<class_Resource_property_resource_local_to_scene>`) |
   +-------------------------+-------------------------+---------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                                        | :ref:`get_current_length<class_AnimationNodeStateMachinePlayback_method_get_current_length>`\ (\ ) |const|                                                                    |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`StringName<class_StringName>`                              | :ref:`get_current_node<class_AnimationNodeStateMachinePlayback_method_get_current_node>`\ (\ ) |const|                                                                        |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                                        | :ref:`get_current_play_position<class_AnimationNodeStateMachinePlayback_method_get_current_play_position>`\ (\ ) |const|                                                      |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`StringName<class_StringName>`                              | :ref:`get_fading_from_node<class_AnimationNodeStateMachinePlayback_method_get_fading_from_node>`\ (\ ) |const|                                                                |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Array<class_Array>`\[:ref:`StringName<class_StringName>`\] | :ref:`get_travel_path<class_AnimationNodeStateMachinePlayback_method_get_travel_path>`\ (\ ) |const|                                                                          |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                                          | :ref:`is_playing<class_AnimationNodeStateMachinePlayback_method_is_playing>`\ (\ ) |const|                                                                                    |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                           | :ref:`next<class_AnimationNodeStateMachinePlayback_method_next>`\ (\ )                                                                                                        |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                           | :ref:`start<class_AnimationNodeStateMachinePlayback_method_start>`\ (\ node\: :ref:`StringName<class_StringName>`, reset\: :ref:`bool<class_bool>` = true\ )                  |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                           | :ref:`stop<class_AnimationNodeStateMachinePlayback_method_stop>`\ (\ )                                                                                                        |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                                           | :ref:`travel<class_AnimationNodeStateMachinePlayback_method_travel>`\ (\ to_node\: :ref:`StringName<class_StringName>`, reset_on_teleport\: :ref:`bool<class_bool>` = true\ ) |
   +------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_AnimationNodeStateMachinePlayback_signal_state_finished:

.. rst-class:: classref-signal

**state_finished**\ (\ state\: :ref:`StringName<class_StringName>`\ ) :ref:`🔗<class_AnimationNodeStateMachinePlayback_signal_state_finished>`

Emitted when the ``state`` finishes playback. If ``state`` is a state machine set to grouped mode, its signals are passed through with its name prefixed.

If there is a crossfade, this will be fired when the influence of the :ref:`get_fading_from_node()<class_AnimationNodeStateMachinePlayback_method_get_fading_from_node>` animation is no longer present.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_signal_state_started:

.. rst-class:: classref-signal

**state_started**\ (\ state\: :ref:`StringName<class_StringName>`\ ) :ref:`🔗<class_AnimationNodeStateMachinePlayback_signal_state_started>`

Emitted when the ``state`` starts playback. If ``state`` is a state machine set to grouped mode, its signals are passed through with its name prefixed.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_AnimationNodeStateMachinePlayback_method_get_current_length:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_current_length**\ (\ ) |const| :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_get_current_length>`

Returns the current state length.

\ **Note:** It is possible that any :ref:`AnimationRootNode<class_AnimationRootNode>` can be nodes as well as animations. This means that there can be multiple animations within a single state. Which animation length has priority depends on the nodes connected inside it. Also, if a transition does not reset, the remaining length at that point will be returned.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_get_current_node:

.. rst-class:: classref-method

:ref:`StringName<class_StringName>` **get_current_node**\ (\ ) |const| :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_get_current_node>`

Returns the currently playing animation state.

\ **Note:** When using a cross-fade, the current state changes to the next state immediately after the cross-fade begins.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_get_current_play_position:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_current_play_position**\ (\ ) |const| :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_get_current_play_position>`

Returns the playback position within the current animation state.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_get_fading_from_node:

.. rst-class:: classref-method

:ref:`StringName<class_StringName>` **get_fading_from_node**\ (\ ) |const| :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_get_fading_from_node>`

Returns the starting state of currently fading animation.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_get_travel_path:

.. rst-class:: classref-method

:ref:`Array<class_Array>`\[:ref:`StringName<class_StringName>`\] **get_travel_path**\ (\ ) |const| :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_get_travel_path>`

Returns the current travel path as computed internally by the A\* algorithm.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_is_playing:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_playing**\ (\ ) |const| :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_is_playing>`

Returns ``true`` if an animation is playing.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_next:

.. rst-class:: classref-method

|void| **next**\ (\ ) :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_next>`

If there is a next path by travel or auto advance, immediately transitions from the current state to the next state.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_start:

.. rst-class:: classref-method

|void| **start**\ (\ node\: :ref:`StringName<class_StringName>`, reset\: :ref:`bool<class_bool>` = true\ ) :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_start>`

Starts playing the given animation.

If ``reset`` is ``true``, the animation is played from the beginning.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_stop:

.. rst-class:: classref-method

|void| **stop**\ (\ ) :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_stop>`

Stops the currently playing animation.

.. rst-class:: classref-item-separator

----

.. _class_AnimationNodeStateMachinePlayback_method_travel:

.. rst-class:: classref-method

|void| **travel**\ (\ to_node\: :ref:`StringName<class_StringName>`, reset_on_teleport\: :ref:`bool<class_bool>` = true\ ) :ref:`🔗<class_AnimationNodeStateMachinePlayback_method_travel>`

Transitions from the current state to another one, following the shortest path.

If the path does not connect from the current state, the animation will play after the state teleports.

If ``reset_on_teleport`` is ``true``, the animation is played from the beginning when the travel cause a teleportation.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
