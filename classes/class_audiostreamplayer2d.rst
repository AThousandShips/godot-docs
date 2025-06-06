:github_url: hide

.. meta::
	:keywords: sound, sfx

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/AudioStreamPlayer2D.xml.

.. _class_AudioStreamPlayer2D:

AudioStreamPlayer2D
===================

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Plays positional sound in 2D space.

.. rst-class:: classref-introduction-group

Description
-----------

Plays audio that is attenuated with distance to the listener.

By default, audio is heard from the screen center. This can be changed by adding an :ref:`AudioListener2D<class_AudioListener2D>` node to the scene and enabling it by calling :ref:`AudioListener2D.make_current()<class_AudioListener2D_method_make_current>` on it.

See also :ref:`AudioStreamPlayer<class_AudioStreamPlayer>` to play a sound non-positionally.

\ **Note:** Hiding an **AudioStreamPlayer2D** node does not disable its audio output. To temporarily disable an **AudioStreamPlayer2D**'s audio output, set :ref:`volume_db<class_AudioStreamPlayer2D_property_volume_db>` to a very low value like ``-100`` (which isn't audible to human hearing).

.. rst-class:: classref-introduction-group

Tutorials
---------

- :doc:`Audio streams <../tutorials/audio/audio_streams>`

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`int<class_int>`                              | :ref:`area_mask<class_AudioStreamPlayer2D_property_area_mask>`               | ``1``         |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`attenuation<class_AudioStreamPlayer2D_property_attenuation>`           | ``1.0``       |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`bool<class_bool>`                            | :ref:`autoplay<class_AudioStreamPlayer2D_property_autoplay>`                 | ``false``     |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`StringName<class_StringName>`                | :ref:`bus<class_AudioStreamPlayer2D_property_bus>`                           | ``&"Master"`` |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`max_distance<class_AudioStreamPlayer2D_property_max_distance>`         | ``2000.0``    |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`int<class_int>`                              | :ref:`max_polyphony<class_AudioStreamPlayer2D_property_max_polyphony>`       | ``1``         |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`panning_strength<class_AudioStreamPlayer2D_property_panning_strength>` | ``1.0``       |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`pitch_scale<class_AudioStreamPlayer2D_property_pitch_scale>`           | ``1.0``       |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`PlaybackType<enum_AudioServer_PlaybackType>` | :ref:`playback_type<class_AudioStreamPlayer2D_property_playback_type>`       | ``0``         |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`bool<class_bool>`                            | :ref:`playing<class_AudioStreamPlayer2D_property_playing>`                   | ``false``     |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`AudioStream<class_AudioStream>`              | :ref:`stream<class_AudioStreamPlayer2D_property_stream>`                     |               |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`bool<class_bool>`                            | :ref:`stream_paused<class_AudioStreamPlayer2D_property_stream_paused>`       | ``false``     |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`volume_db<class_AudioStreamPlayer2D_property_volume_db>`               | ``0.0``       |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`volume_linear<class_AudioStreamPlayer2D_property_volume_linear>`       |               |
   +----------------------------------------------------+------------------------------------------------------------------------------+---------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                             | :ref:`get_playback_position<class_AudioStreamPlayer2D_method_get_playback_position>`\ (\ )                |
   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` | :ref:`get_stream_playback<class_AudioStreamPlayer2D_method_get_stream_playback>`\ (\ )                    |
   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | :ref:`has_stream_playback<class_AudioStreamPlayer2D_method_has_stream_playback>`\ (\ )                    |
   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | |void|                                                | :ref:`play<class_AudioStreamPlayer2D_method_play>`\ (\ from_position\: :ref:`float<class_float>` = 0.0\ ) |
   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | |void|                                                | :ref:`seek<class_AudioStreamPlayer2D_method_seek>`\ (\ to_position\: :ref:`float<class_float>`\ )         |
   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | |void|                                                | :ref:`stop<class_AudioStreamPlayer2D_method_stop>`\ (\ )                                                  |
   +-------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_AudioStreamPlayer2D_signal_finished:

.. rst-class:: classref-signal

**finished**\ (\ ) :ref:`🔗<class_AudioStreamPlayer2D_signal_finished>`

Emitted when the audio stops playing.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_AudioStreamPlayer2D_property_area_mask:

.. rst-class:: classref-property

:ref:`int<class_int>` **area_mask** = ``1`` :ref:`🔗<class_AudioStreamPlayer2D_property_area_mask>`

.. rst-class:: classref-property-setget

- |void| **set_area_mask**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_area_mask**\ (\ )

Determines which :ref:`Area2D<class_Area2D>` layers affect the sound for reverb and audio bus effects. Areas can be used to redirect :ref:`AudioStream<class_AudioStream>`\ s so that they play in a certain audio bus. An example of how you might use this is making a "water" area so that sounds played in the water are redirected through an audio bus to make them sound like they are being played underwater.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_attenuation:

.. rst-class:: classref-property

:ref:`float<class_float>` **attenuation** = ``1.0`` :ref:`🔗<class_AudioStreamPlayer2D_property_attenuation>`

.. rst-class:: classref-property-setget

- |void| **set_attenuation**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_attenuation**\ (\ )

The volume is attenuated over distance with this as an exponent.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_autoplay:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **autoplay** = ``false`` :ref:`🔗<class_AudioStreamPlayer2D_property_autoplay>`

.. rst-class:: classref-property-setget

- |void| **set_autoplay**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_autoplay_enabled**\ (\ )

If ``true``, audio plays when added to scene tree.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_bus:

.. rst-class:: classref-property

:ref:`StringName<class_StringName>` **bus** = ``&"Master"`` :ref:`🔗<class_AudioStreamPlayer2D_property_bus>`

.. rst-class:: classref-property-setget

- |void| **set_bus**\ (\ value\: :ref:`StringName<class_StringName>`\ )
- :ref:`StringName<class_StringName>` **get_bus**\ (\ )

Bus on which this audio is playing.

\ **Note:** When setting this property, keep in mind that no validation is performed to see if the given name matches an existing bus. This is because audio bus layouts might be loaded after this property is set. If this given name can't be resolved at runtime, it will fall back to ``"Master"``.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_max_distance:

.. rst-class:: classref-property

:ref:`float<class_float>` **max_distance** = ``2000.0`` :ref:`🔗<class_AudioStreamPlayer2D_property_max_distance>`

.. rst-class:: classref-property-setget

- |void| **set_max_distance**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_max_distance**\ (\ )

Maximum distance from which audio is still hearable.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_max_polyphony:

.. rst-class:: classref-property

:ref:`int<class_int>` **max_polyphony** = ``1`` :ref:`🔗<class_AudioStreamPlayer2D_property_max_polyphony>`

.. rst-class:: classref-property-setget

- |void| **set_max_polyphony**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_max_polyphony**\ (\ )

The maximum number of sounds this node can play at the same time. Playing additional sounds after this value is reached will cut off the oldest sounds.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_panning_strength:

.. rst-class:: classref-property

:ref:`float<class_float>` **panning_strength** = ``1.0`` :ref:`🔗<class_AudioStreamPlayer2D_property_panning_strength>`

.. rst-class:: classref-property-setget

- |void| **set_panning_strength**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_panning_strength**\ (\ )

Scales the panning strength for this node by multiplying the base :ref:`ProjectSettings.audio/general/2d_panning_strength<class_ProjectSettings_property_audio/general/2d_panning_strength>` with this factor. Higher values will pan audio from left to right more dramatically than lower values.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_pitch_scale:

.. rst-class:: classref-property

:ref:`float<class_float>` **pitch_scale** = ``1.0`` :ref:`🔗<class_AudioStreamPlayer2D_property_pitch_scale>`

.. rst-class:: classref-property-setget

- |void| **set_pitch_scale**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_pitch_scale**\ (\ )

The pitch and the tempo of the audio, as a multiplier of the audio sample's sample rate.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_playback_type:

.. rst-class:: classref-property

:ref:`PlaybackType<enum_AudioServer_PlaybackType>` **playback_type** = ``0`` :ref:`🔗<class_AudioStreamPlayer2D_property_playback_type>`

.. rst-class:: classref-property-setget

- |void| **set_playback_type**\ (\ value\: :ref:`PlaybackType<enum_AudioServer_PlaybackType>`\ )
- :ref:`PlaybackType<enum_AudioServer_PlaybackType>` **get_playback_type**\ (\ )

**Experimental:** This property may be changed or removed in future versions.

The playback type of the stream player. If set other than to the default value, it will force that playback type.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_playing:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **playing** = ``false`` :ref:`🔗<class_AudioStreamPlayer2D_property_playing>`

.. rst-class:: classref-property-setget

- |void| **set_playing**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_playing**\ (\ )

If ``true``, audio is playing or is queued to be played (see :ref:`play()<class_AudioStreamPlayer2D_method_play>`).

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_stream:

.. rst-class:: classref-property

:ref:`AudioStream<class_AudioStream>` **stream** :ref:`🔗<class_AudioStreamPlayer2D_property_stream>`

.. rst-class:: classref-property-setget

- |void| **set_stream**\ (\ value\: :ref:`AudioStream<class_AudioStream>`\ )
- :ref:`AudioStream<class_AudioStream>` **get_stream**\ (\ )

The :ref:`AudioStream<class_AudioStream>` object to be played.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_stream_paused:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **stream_paused** = ``false`` :ref:`🔗<class_AudioStreamPlayer2D_property_stream_paused>`

.. rst-class:: classref-property-setget

- |void| **set_stream_paused**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **get_stream_paused**\ (\ )

If ``true``, the playback is paused. You can resume it by setting :ref:`stream_paused<class_AudioStreamPlayer2D_property_stream_paused>` to ``false``.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_volume_db:

.. rst-class:: classref-property

:ref:`float<class_float>` **volume_db** = ``0.0`` :ref:`🔗<class_AudioStreamPlayer2D_property_volume_db>`

.. rst-class:: classref-property-setget

- |void| **set_volume_db**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_volume_db**\ (\ )

Base volume before attenuation, in decibels.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_property_volume_linear:

.. rst-class:: classref-property

:ref:`float<class_float>` **volume_linear** :ref:`🔗<class_AudioStreamPlayer2D_property_volume_linear>`

.. rst-class:: classref-property-setget

- |void| **set_volume_linear**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_volume_linear**\ (\ )

Base volume before attenuation, as a linear value.

\ **Note:** This member modifies :ref:`volume_db<class_AudioStreamPlayer2D_property_volume_db>` for convenience. The returned value is equivalent to the result of :ref:`@GlobalScope.db_to_linear()<class_@GlobalScope_method_db_to_linear>` on :ref:`volume_db<class_AudioStreamPlayer2D_property_volume_db>`. Setting this member is equivalent to setting :ref:`volume_db<class_AudioStreamPlayer2D_property_volume_db>` to the result of :ref:`@GlobalScope.linear_to_db()<class_@GlobalScope_method_linear_to_db>` on a value.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_AudioStreamPlayer2D_method_get_playback_position:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_playback_position**\ (\ ) :ref:`🔗<class_AudioStreamPlayer2D_method_get_playback_position>`

Returns the position in the :ref:`AudioStream<class_AudioStream>`.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_method_get_stream_playback:

.. rst-class:: classref-method

:ref:`AudioStreamPlayback<class_AudioStreamPlayback>` **get_stream_playback**\ (\ ) :ref:`🔗<class_AudioStreamPlayer2D_method_get_stream_playback>`

Returns the :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` object associated with this **AudioStreamPlayer2D**.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_method_has_stream_playback:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has_stream_playback**\ (\ ) :ref:`🔗<class_AudioStreamPlayer2D_method_has_stream_playback>`

Returns whether the :ref:`AudioStreamPlayer<class_AudioStreamPlayer>` can return the :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` object or not.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_method_play:

.. rst-class:: classref-method

|void| **play**\ (\ from_position\: :ref:`float<class_float>` = 0.0\ ) :ref:`🔗<class_AudioStreamPlayer2D_method_play>`

Queues the audio to play on the next physics frame, from the given position ``from_position``, in seconds.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_method_seek:

.. rst-class:: classref-method

|void| **seek**\ (\ to_position\: :ref:`float<class_float>`\ ) :ref:`🔗<class_AudioStreamPlayer2D_method_seek>`

Sets the position from which audio will be played, in seconds.

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer2D_method_stop:

.. rst-class:: classref-method

|void| **stop**\ (\ ) :ref:`🔗<class_AudioStreamPlayer2D_method_stop>`

Stops the audio.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
