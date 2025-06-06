:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/StyleBoxFlat.xml.

.. _class_StyleBoxFlat:

StyleBoxFlat
============

**Inherits:** :ref:`StyleBox<class_StyleBox>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A customizable :ref:`StyleBox<class_StyleBox>` that doesn't use a texture.

.. rst-class:: classref-introduction-group

Description
-----------

By configuring various properties of this style box, you can achieve many common looks without the need of a texture. This includes optionally rounded borders, antialiasing, shadows, and skew.

Setting corner radius to high values is allowed. As soon as corners overlap, the stylebox will switch to a relative system:

.. code:: text

    height = 30
    corner_radius_top_left = 50
    corner_radius_bottom_left = 100

The relative system now would take the 1:2 ratio of the two left corners to calculate the actual corner width. Both corners added will **never** be more than the height. Result:

.. code:: text

    corner_radius_top_left: 10
    corner_radius_bottom_left: 20

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`bool<class_bool>`       | :ref:`anti_aliasing<class_StyleBoxFlat_property_anti_aliasing>`                           | ``true``                    |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`float<class_float>`     | :ref:`anti_aliasing_size<class_StyleBoxFlat_property_anti_aliasing_size>`                 | ``1.0``                     |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`Color<class_Color>`     | :ref:`bg_color<class_StyleBoxFlat_property_bg_color>`                                     | ``Color(0.6, 0.6, 0.6, 1)`` |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`bool<class_bool>`       | :ref:`border_blend<class_StyleBoxFlat_property_border_blend>`                             | ``false``                   |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`Color<class_Color>`     | :ref:`border_color<class_StyleBoxFlat_property_border_color>`                             | ``Color(0.8, 0.8, 0.8, 1)`` |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`border_width_bottom<class_StyleBoxFlat_property_border_width_bottom>`               | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`border_width_left<class_StyleBoxFlat_property_border_width_left>`                   | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`border_width_right<class_StyleBoxFlat_property_border_width_right>`                 | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`border_width_top<class_StyleBoxFlat_property_border_width_top>`                     | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`corner_detail<class_StyleBoxFlat_property_corner_detail>`                           | ``8``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`corner_radius_bottom_left<class_StyleBoxFlat_property_corner_radius_bottom_left>`   | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`corner_radius_bottom_right<class_StyleBoxFlat_property_corner_radius_bottom_right>` | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`corner_radius_top_left<class_StyleBoxFlat_property_corner_radius_top_left>`         | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`corner_radius_top_right<class_StyleBoxFlat_property_corner_radius_top_right>`       | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`bool<class_bool>`       | :ref:`draw_center<class_StyleBoxFlat_property_draw_center>`                               | ``true``                    |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`float<class_float>`     | :ref:`expand_margin_bottom<class_StyleBoxFlat_property_expand_margin_bottom>`             | ``0.0``                     |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`float<class_float>`     | :ref:`expand_margin_left<class_StyleBoxFlat_property_expand_margin_left>`                 | ``0.0``                     |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`float<class_float>`     | :ref:`expand_margin_right<class_StyleBoxFlat_property_expand_margin_right>`               | ``0.0``                     |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`float<class_float>`     | :ref:`expand_margin_top<class_StyleBoxFlat_property_expand_margin_top>`                   | ``0.0``                     |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`Color<class_Color>`     | :ref:`shadow_color<class_StyleBoxFlat_property_shadow_color>`                             | ``Color(0, 0, 0, 0.6)``     |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`shadow_offset<class_StyleBoxFlat_property_shadow_offset>`                           | ``Vector2(0, 0)``           |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`int<class_int>`         | :ref:`shadow_size<class_StyleBoxFlat_property_shadow_size>`                               | ``0``                       |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`skew<class_StyleBoxFlat_property_skew>`                                             | ``Vector2(0, 0)``           |
   +-------------------------------+-------------------------------------------------------------------------------------------+-----------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`     | :ref:`get_border_width<class_StyleBoxFlat_method_get_border_width>`\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|                               |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`     | :ref:`get_border_width_min<class_StyleBoxFlat_method_get_border_width_min>`\ (\ ) |const|                                                                     |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`     | :ref:`get_corner_radius<class_StyleBoxFlat_method_get_corner_radius>`\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`\ ) |const|                         |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`get_expand_margin<class_StyleBoxFlat_method_get_expand_margin>`\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|                             |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`set_border_width<class_StyleBoxFlat_method_set_border_width>`\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, width\: :ref:`int<class_int>`\ )        |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`set_border_width_all<class_StyleBoxFlat_method_set_border_width_all>`\ (\ width\: :ref:`int<class_int>`\ )                                              |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`set_corner_radius<class_StyleBoxFlat_method_set_corner_radius>`\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`, radius\: :ref:`int<class_int>`\ ) |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`set_corner_radius_all<class_StyleBoxFlat_method_set_corner_radius_all>`\ (\ radius\: :ref:`int<class_int>`\ )                                           |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`set_expand_margin<class_StyleBoxFlat_method_set_expand_margin>`\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, size\: :ref:`float<class_float>`\ )   |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                    | :ref:`set_expand_margin_all<class_StyleBoxFlat_method_set_expand_margin_all>`\ (\ size\: :ref:`float<class_float>`\ )                                         |
   +---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_StyleBoxFlat_property_anti_aliasing:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **anti_aliasing** = ``true`` :ref:`🔗<class_StyleBoxFlat_property_anti_aliasing>`

.. rst-class:: classref-property-setget

- |void| **set_anti_aliased**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_anti_aliased**\ (\ )

Antialiasing draws a small ring around the edges, which fades to transparency. As a result, edges look much smoother. This is only noticeable when using rounded corners or :ref:`skew<class_StyleBoxFlat_property_skew>`.

\ **Note:** When using beveled corners with 45-degree angles (:ref:`corner_detail<class_StyleBoxFlat_property_corner_detail>` = 1), it is recommended to set :ref:`anti_aliasing<class_StyleBoxFlat_property_anti_aliasing>` to ``false`` to ensure crisp visuals and avoid possible visual glitches.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_anti_aliasing_size:

.. rst-class:: classref-property

:ref:`float<class_float>` **anti_aliasing_size** = ``1.0`` :ref:`🔗<class_StyleBoxFlat_property_anti_aliasing_size>`

.. rst-class:: classref-property-setget

- |void| **set_aa_size**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_aa_size**\ (\ )

This changes the size of the antialiasing effect. ``1.0`` is recommended for an optimal result at 100% scale, identical to how rounded rectangles are rendered in web browsers and most vector drawing software.

\ **Note:** Higher values may produce a blur effect but can also create undesired artifacts on small boxes with large-radius corners.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_bg_color:

.. rst-class:: classref-property

:ref:`Color<class_Color>` **bg_color** = ``Color(0.6, 0.6, 0.6, 1)`` :ref:`🔗<class_StyleBoxFlat_property_bg_color>`

.. rst-class:: classref-property-setget

- |void| **set_bg_color**\ (\ value\: :ref:`Color<class_Color>`\ )
- :ref:`Color<class_Color>` **get_bg_color**\ (\ )

The background color of the stylebox.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_border_blend:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **border_blend** = ``false`` :ref:`🔗<class_StyleBoxFlat_property_border_blend>`

.. rst-class:: classref-property-setget

- |void| **set_border_blend**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **get_border_blend**\ (\ )

If ``true``, the border will fade into the background color.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_border_color:

.. rst-class:: classref-property

:ref:`Color<class_Color>` **border_color** = ``Color(0.8, 0.8, 0.8, 1)`` :ref:`🔗<class_StyleBoxFlat_property_border_color>`

.. rst-class:: classref-property-setget

- |void| **set_border_color**\ (\ value\: :ref:`Color<class_Color>`\ )
- :ref:`Color<class_Color>` **get_border_color**\ (\ )

Sets the color of the border.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_border_width_bottom:

.. rst-class:: classref-property

:ref:`int<class_int>` **border_width_bottom** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_border_width_bottom>`

.. rst-class:: classref-property-setget

- |void| **set_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, width\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Border width for the bottom border.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_border_width_left:

.. rst-class:: classref-property

:ref:`int<class_int>` **border_width_left** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_border_width_left>`

.. rst-class:: classref-property-setget

- |void| **set_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, width\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Border width for the left border.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_border_width_right:

.. rst-class:: classref-property

:ref:`int<class_int>` **border_width_right** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_border_width_right>`

.. rst-class:: classref-property-setget

- |void| **set_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, width\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Border width for the right border.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_border_width_top:

.. rst-class:: classref-property

:ref:`int<class_int>` **border_width_top** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_border_width_top>`

.. rst-class:: classref-property-setget

- |void| **set_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, width\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Border width for the top border.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_corner_detail:

.. rst-class:: classref-property

:ref:`int<class_int>` **corner_detail** = ``8`` :ref:`🔗<class_StyleBoxFlat_property_corner_detail>`

.. rst-class:: classref-property-setget

- |void| **set_corner_detail**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_corner_detail**\ (\ )

This sets the number of vertices used for each corner. Higher values result in rounder corners but take more processing power to compute. When choosing a value, you should take the corner radius (:ref:`set_corner_radius_all()<class_StyleBoxFlat_method_set_corner_radius_all>`) into account.

For corner radii less than 10, ``4`` or ``5`` should be enough. For corner radii less than 30, values between ``8`` and ``12`` should be enough.

A corner detail of ``1`` will result in chamfered corners instead of rounded corners, which is useful for some artistic effects.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_corner_radius_bottom_left:

.. rst-class:: classref-property

:ref:`int<class_int>` **corner_radius_bottom_left** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_corner_radius_bottom_left>`

.. rst-class:: classref-property-setget

- |void| **set_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`, radius\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`\ ) |const|

The bottom-left corner's radius. If ``0``, the corner is not rounded.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_corner_radius_bottom_right:

.. rst-class:: classref-property

:ref:`int<class_int>` **corner_radius_bottom_right** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_corner_radius_bottom_right>`

.. rst-class:: classref-property-setget

- |void| **set_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`, radius\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`\ ) |const|

The bottom-right corner's radius. If ``0``, the corner is not rounded.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_corner_radius_top_left:

.. rst-class:: classref-property

:ref:`int<class_int>` **corner_radius_top_left** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_corner_radius_top_left>`

.. rst-class:: classref-property-setget

- |void| **set_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`, radius\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`\ ) |const|

The top-left corner's radius. If ``0``, the corner is not rounded.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_corner_radius_top_right:

.. rst-class:: classref-property

:ref:`int<class_int>` **corner_radius_top_right** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_corner_radius_top_right>`

.. rst-class:: classref-property-setget

- |void| **set_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`, radius\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`\ ) |const|

The top-right corner's radius. If ``0``, the corner is not rounded.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_draw_center:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **draw_center** = ``true`` :ref:`🔗<class_StyleBoxFlat_property_draw_center>`

.. rst-class:: classref-property-setget

- |void| **set_draw_center**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_draw_center_enabled**\ (\ )

Toggles drawing of the inner part of the stylebox.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_expand_margin_bottom:

.. rst-class:: classref-property

:ref:`float<class_float>` **expand_margin_bottom** = ``0.0`` :ref:`🔗<class_StyleBoxFlat_property_expand_margin_bottom>`

.. rst-class:: classref-property-setget

- |void| **set_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, size\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Expands the stylebox outside of the control rect on the bottom edge. Useful in combination with :ref:`border_width_bottom<class_StyleBoxFlat_property_border_width_bottom>` to draw a border outside the control rect.

\ **Note:** Unlike :ref:`StyleBox.content_margin_bottom<class_StyleBox_property_content_margin_bottom>`, :ref:`expand_margin_bottom<class_StyleBoxFlat_property_expand_margin_bottom>` does *not* affect the size of the clickable area for :ref:`Control<class_Control>`\ s. This can negatively impact usability if used wrong, as the user may try to click an area of the StyleBox that cannot actually receive clicks.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_expand_margin_left:

.. rst-class:: classref-property

:ref:`float<class_float>` **expand_margin_left** = ``0.0`` :ref:`🔗<class_StyleBoxFlat_property_expand_margin_left>`

.. rst-class:: classref-property-setget

- |void| **set_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, size\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Expands the stylebox outside of the control rect on the left edge. Useful in combination with :ref:`border_width_left<class_StyleBoxFlat_property_border_width_left>` to draw a border outside the control rect.

\ **Note:** Unlike :ref:`StyleBox.content_margin_left<class_StyleBox_property_content_margin_left>`, :ref:`expand_margin_left<class_StyleBoxFlat_property_expand_margin_left>` does *not* affect the size of the clickable area for :ref:`Control<class_Control>`\ s. This can negatively impact usability if used wrong, as the user may try to click an area of the StyleBox that cannot actually receive clicks.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_expand_margin_right:

.. rst-class:: classref-property

:ref:`float<class_float>` **expand_margin_right** = ``0.0`` :ref:`🔗<class_StyleBoxFlat_property_expand_margin_right>`

.. rst-class:: classref-property-setget

- |void| **set_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, size\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Expands the stylebox outside of the control rect on the right edge. Useful in combination with :ref:`border_width_right<class_StyleBoxFlat_property_border_width_right>` to draw a border outside the control rect.

\ **Note:** Unlike :ref:`StyleBox.content_margin_right<class_StyleBox_property_content_margin_right>`, :ref:`expand_margin_right<class_StyleBoxFlat_property_expand_margin_right>` does *not* affect the size of the clickable area for :ref:`Control<class_Control>`\ s. This can negatively impact usability if used wrong, as the user may try to click an area of the StyleBox that cannot actually receive clicks.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_expand_margin_top:

.. rst-class:: classref-property

:ref:`float<class_float>` **expand_margin_top** = ``0.0`` :ref:`🔗<class_StyleBoxFlat_property_expand_margin_top>`

.. rst-class:: classref-property-setget

- |void| **set_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, size\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const|

Expands the stylebox outside of the control rect on the top edge. Useful in combination with :ref:`border_width_top<class_StyleBoxFlat_property_border_width_top>` to draw a border outside the control rect.

\ **Note:** Unlike :ref:`StyleBox.content_margin_top<class_StyleBox_property_content_margin_top>`, :ref:`expand_margin_top<class_StyleBoxFlat_property_expand_margin_top>` does *not* affect the size of the clickable area for :ref:`Control<class_Control>`\ s. This can negatively impact usability if used wrong, as the user may try to click an area of the StyleBox that cannot actually receive clicks.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_shadow_color:

.. rst-class:: classref-property

:ref:`Color<class_Color>` **shadow_color** = ``Color(0, 0, 0, 0.6)`` :ref:`🔗<class_StyleBoxFlat_property_shadow_color>`

.. rst-class:: classref-property-setget

- |void| **set_shadow_color**\ (\ value\: :ref:`Color<class_Color>`\ )
- :ref:`Color<class_Color>` **get_shadow_color**\ (\ )

The color of the shadow. This has no effect if :ref:`shadow_size<class_StyleBoxFlat_property_shadow_size>` is lower than 1.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_shadow_offset:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **shadow_offset** = ``Vector2(0, 0)`` :ref:`🔗<class_StyleBoxFlat_property_shadow_offset>`

.. rst-class:: classref-property-setget

- |void| **set_shadow_offset**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_shadow_offset**\ (\ )

The shadow offset in pixels. Adjusts the position of the shadow relatively to the stylebox.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_shadow_size:

.. rst-class:: classref-property

:ref:`int<class_int>` **shadow_size** = ``0`` :ref:`🔗<class_StyleBoxFlat_property_shadow_size>`

.. rst-class:: classref-property-setget

- |void| **set_shadow_size**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_shadow_size**\ (\ )

The shadow size in pixels.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_property_skew:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **skew** = ``Vector2(0, 0)`` :ref:`🔗<class_StyleBoxFlat_property_skew>`

.. rst-class:: classref-property-setget

- |void| **set_skew**\ (\ value\: :ref:`Vector2<class_Vector2>`\ )
- :ref:`Vector2<class_Vector2>` **get_skew**\ (\ )

If set to a non-zero value on either axis, :ref:`skew<class_StyleBoxFlat_property_skew>` distorts the StyleBox horizontally and/or vertically. This can be used for "futuristic"-style UIs. Positive values skew the StyleBox towards the right (X axis) and upwards (Y axis), while negative values skew the StyleBox towards the left (X axis) and downwards (Y axis).

\ **Note:** To ensure text does not touch the StyleBox's edges, consider increasing the :ref:`StyleBox<class_StyleBox>`'s content margin (see :ref:`StyleBox.content_margin_bottom<class_StyleBox_property_content_margin_bottom>`). It is preferable to increase the content margin instead of the expand margin (see :ref:`expand_margin_bottom<class_StyleBoxFlat_property_expand_margin_bottom>`), as increasing the expand margin does not increase the size of the clickable area for :ref:`Control<class_Control>`\ s.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_StyleBoxFlat_method_get_border_width:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const| :ref:`🔗<class_StyleBoxFlat_method_get_border_width>`

Returns the specified :ref:`Side<enum_@GlobalScope_Side>`'s border width.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_get_border_width_min:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_border_width_min**\ (\ ) |const| :ref:`🔗<class_StyleBoxFlat_method_get_border_width_min>`

Returns the smallest border width out of all four borders.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_get_corner_radius:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`\ ) |const| :ref:`🔗<class_StyleBoxFlat_method_get_corner_radius>`

Returns the given ``corner``'s radius.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_get_expand_margin:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`\ ) |const| :ref:`🔗<class_StyleBoxFlat_method_get_expand_margin>`

Returns the size of the specified :ref:`Side<enum_@GlobalScope_Side>`'s expand margin.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_set_border_width:

.. rst-class:: classref-method

|void| **set_border_width**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, width\: :ref:`int<class_int>`\ ) :ref:`🔗<class_StyleBoxFlat_method_set_border_width>`

Sets the specified :ref:`Side<enum_@GlobalScope_Side>`'s border width to ``width`` pixels.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_set_border_width_all:

.. rst-class:: classref-method

|void| **set_border_width_all**\ (\ width\: :ref:`int<class_int>`\ ) :ref:`🔗<class_StyleBoxFlat_method_set_border_width_all>`

Sets the border width to ``width`` pixels for all sides.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_set_corner_radius:

.. rst-class:: classref-method

|void| **set_corner_radius**\ (\ corner\: :ref:`Corner<enum_@GlobalScope_Corner>`, radius\: :ref:`int<class_int>`\ ) :ref:`🔗<class_StyleBoxFlat_method_set_corner_radius>`

Sets the corner radius to ``radius`` pixels for the given ``corner``.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_set_corner_radius_all:

.. rst-class:: classref-method

|void| **set_corner_radius_all**\ (\ radius\: :ref:`int<class_int>`\ ) :ref:`🔗<class_StyleBoxFlat_method_set_corner_radius_all>`

Sets the corner radius to ``radius`` pixels for all corners.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_set_expand_margin:

.. rst-class:: classref-method

|void| **set_expand_margin**\ (\ margin\: :ref:`Side<enum_@GlobalScope_Side>`, size\: :ref:`float<class_float>`\ ) :ref:`🔗<class_StyleBoxFlat_method_set_expand_margin>`

Sets the expand margin to ``size`` pixels for the specified :ref:`Side<enum_@GlobalScope_Side>`.

.. rst-class:: classref-item-separator

----

.. _class_StyleBoxFlat_method_set_expand_margin_all:

.. rst-class:: classref-method

|void| **set_expand_margin_all**\ (\ size\: :ref:`float<class_float>`\ ) :ref:`🔗<class_StyleBoxFlat_method_set_expand_margin_all>`

Sets the expand margin to ``size`` pixels for all sides.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
