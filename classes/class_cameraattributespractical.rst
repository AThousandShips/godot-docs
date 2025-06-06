:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/CameraAttributesPractical.xml.

.. _class_CameraAttributesPractical:

CameraAttributesPractical
=========================

**Inherits:** :ref:`CameraAttributes<class_CameraAttributes>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Camera settings in an easy to use format.

.. rst-class:: classref-introduction-group

Description
-----------

Controls camera-specific attributes such as auto-exposure, depth of field, and exposure override.

When used in a :ref:`WorldEnvironment<class_WorldEnvironment>` it provides default settings for exposure, auto-exposure, and depth of field that will be used by all cameras without their own :ref:`CameraAttributes<class_CameraAttributes>`, including the editor camera. When used in a :ref:`Camera3D<class_Camera3D>` it will override any :ref:`CameraAttributes<class_CameraAttributes>` set in the :ref:`WorldEnvironment<class_WorldEnvironment>`. When used in :ref:`VoxelGI<class_VoxelGI>` or :ref:`LightmapGI<class_LightmapGI>`, only the exposure settings will be used.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`auto_exposure_max_sensitivity<class_CameraAttributesPractical_property_auto_exposure_max_sensitivity>` | ``800.0`` |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`auto_exposure_min_sensitivity<class_CameraAttributesPractical_property_auto_exposure_min_sensitivity>` | ``0.0``   |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`dof_blur_amount<class_CameraAttributesPractical_property_dof_blur_amount>`                             | ``0.1``   |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`dof_blur_far_distance<class_CameraAttributesPractical_property_dof_blur_far_distance>`                 | ``10.0``  |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`   | :ref:`dof_blur_far_enabled<class_CameraAttributesPractical_property_dof_blur_far_enabled>`                   | ``false`` |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`dof_blur_far_transition<class_CameraAttributesPractical_property_dof_blur_far_transition>`             | ``5.0``   |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`dof_blur_near_distance<class_CameraAttributesPractical_property_dof_blur_near_distance>`               | ``2.0``   |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`   | :ref:`dof_blur_near_enabled<class_CameraAttributesPractical_property_dof_blur_near_enabled>`                 | ``false`` |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`dof_blur_near_transition<class_CameraAttributesPractical_property_dof_blur_near_transition>`           | ``1.0``   |
   +---------------------------+--------------------------------------------------------------------------------------------------------------+-----------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_CameraAttributesPractical_property_auto_exposure_max_sensitivity:

.. rst-class:: classref-property

:ref:`float<class_float>` **auto_exposure_max_sensitivity** = ``800.0`` :ref:`🔗<class_CameraAttributesPractical_property_auto_exposure_max_sensitivity>`

.. rst-class:: classref-property-setget

- |void| **set_auto_exposure_max_sensitivity**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_auto_exposure_max_sensitivity**\ (\ )

The maximum sensitivity (in ISO) used when calculating auto exposure. When calculating scene average luminance, color values will be clamped to at least this value. This limits the auto-exposure from exposing below a certain brightness, resulting in a cut off point where the scene will remain bright.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_auto_exposure_min_sensitivity:

.. rst-class:: classref-property

:ref:`float<class_float>` **auto_exposure_min_sensitivity** = ``0.0`` :ref:`🔗<class_CameraAttributesPractical_property_auto_exposure_min_sensitivity>`

.. rst-class:: classref-property-setget

- |void| **set_auto_exposure_min_sensitivity**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_auto_exposure_min_sensitivity**\ (\ )

The minimum sensitivity (in ISO) used when calculating auto exposure. When calculating scene average luminance, color values will be clamped to at least this value. This limits the auto-exposure from exposing above a certain brightness, resulting in a cut off point where the scene will remain dark.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_amount:

.. rst-class:: classref-property

:ref:`float<class_float>` **dof_blur_amount** = ``0.1`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_amount>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_amount**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_dof_blur_amount**\ (\ )

Sets the maximum amount of blur. When using physically-based blur amounts, will instead act as a multiplier. High values lead to an increased amount of blurriness, but can be much more expensive to calculate. It is best to keep this as low as possible for a given art style.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_far_distance:

.. rst-class:: classref-property

:ref:`float<class_float>` **dof_blur_far_distance** = ``10.0`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_far_distance>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_far_distance**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_dof_blur_far_distance**\ (\ )

Objects further from the :ref:`Camera3D<class_Camera3D>` by this amount will be blurred by the depth of field effect. Measured in meters.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_far_enabled:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **dof_blur_far_enabled** = ``false`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_far_enabled>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_far_enabled**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_dof_blur_far_enabled**\ (\ )

Enables depth of field blur for objects further than :ref:`dof_blur_far_distance<class_CameraAttributesPractical_property_dof_blur_far_distance>`. Strength of blur is controlled by :ref:`dof_blur_amount<class_CameraAttributesPractical_property_dof_blur_amount>` and modulated by :ref:`dof_blur_far_transition<class_CameraAttributesPractical_property_dof_blur_far_transition>`.

\ **Note:** Depth of field blur is only supported in the Forward+ and Mobile rendering methods, not Compatibility.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_far_transition:

.. rst-class:: classref-property

:ref:`float<class_float>` **dof_blur_far_transition** = ``5.0`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_far_transition>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_far_transition**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_dof_blur_far_transition**\ (\ )

When positive, distance over which (starting from :ref:`dof_blur_far_distance<class_CameraAttributesPractical_property_dof_blur_far_distance>`) blur effect will scale from 0 to :ref:`dof_blur_amount<class_CameraAttributesPractical_property_dof_blur_amount>`. When negative, uses physically-based scaling so depth of field effect will scale from 0 at :ref:`dof_blur_far_distance<class_CameraAttributesPractical_property_dof_blur_far_distance>` and will increase in a physically accurate way as objects get further from the :ref:`Camera3D<class_Camera3D>`.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_near_distance:

.. rst-class:: classref-property

:ref:`float<class_float>` **dof_blur_near_distance** = ``2.0`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_near_distance>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_near_distance**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_dof_blur_near_distance**\ (\ )

Objects closer from the :ref:`Camera3D<class_Camera3D>` by this amount will be blurred by the depth of field effect. Measured in meters.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_near_enabled:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **dof_blur_near_enabled** = ``false`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_near_enabled>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_near_enabled**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_dof_blur_near_enabled**\ (\ )

Enables depth of field blur for objects closer than :ref:`dof_blur_near_distance<class_CameraAttributesPractical_property_dof_blur_near_distance>`. Strength of blur is controlled by :ref:`dof_blur_amount<class_CameraAttributesPractical_property_dof_blur_amount>` and modulated by :ref:`dof_blur_near_transition<class_CameraAttributesPractical_property_dof_blur_near_transition>`.

\ **Note:** Depth of field blur is only supported in the Forward+ and Mobile rendering methods, not Compatibility.

.. rst-class:: classref-item-separator

----

.. _class_CameraAttributesPractical_property_dof_blur_near_transition:

.. rst-class:: classref-property

:ref:`float<class_float>` **dof_blur_near_transition** = ``1.0`` :ref:`🔗<class_CameraAttributesPractical_property_dof_blur_near_transition>`

.. rst-class:: classref-property-setget

- |void| **set_dof_blur_near_transition**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_dof_blur_near_transition**\ (\ )

When positive, distance over which blur effect will scale from 0 to :ref:`dof_blur_amount<class_CameraAttributesPractical_property_dof_blur_amount>`, ending at :ref:`dof_blur_near_distance<class_CameraAttributesPractical_property_dof_blur_near_distance>`. When negative, uses physically-based scaling so depth of field effect will scale from 0 at :ref:`dof_blur_near_distance<class_CameraAttributesPractical_property_dof_blur_near_distance>` and will increase in a physically accurate way as objects get closer to the :ref:`Camera3D<class_Camera3D>`.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
