:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/float.xml.

.. _class_float:

float
=====

A built-in type for floating-point numbers.

.. rst-class:: classref-introduction-group

Description
-----------

The **float** built-in type is a 64-bit double-precision floating-point number, equivalent to ``double`` in C++. This type has 14 reliable decimal digits of precision. The maximum value of **float** is approximately ``1.79769e308``, and the minimum is approximately ``-1.79769e308``.

Many methods and properties in the engine use 32-bit single-precision floating-point numbers instead, equivalent to ``float`` in C++, which have 6 reliable decimal digits of precision. For data structures such as :ref:`Vector2<class_Vector2>` and :ref:`Vector3<class_Vector3>`, Godot uses 32-bit floating-point numbers by default, but it can be changed to use 64-bit doubles if Godot is compiled with the ``precision=double`` option.

Math done using the **float** type is not guaranteed to be exact and will often result in small errors. You should usually use the :ref:`@GlobalScope.is_equal_approx()<class_@GlobalScope_method_is_equal_approx>` and :ref:`@GlobalScope.is_zero_approx()<class_@GlobalScope_method_is_zero_approx>` methods instead of ``==`` to compare **float** values for equality.

.. rst-class:: classref-introduction-group

Tutorials
---------

- `Wikipedia: Double-precision floating-point format <https://en.wikipedia.org/wiki/Double-precision_floating-point_format>`__

- `Wikipedia: Single-precision floating-point format <https://en.wikipedia.org/wiki/Single-precision_floating-point_format>`__

.. rst-class:: classref-reftable-group

Constructors
------------

.. table::
   :widths: auto

   +---------------------------+---------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>`\ (\ )                                     |
   +---------------------------+---------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>`\ (\ from\: :ref:`float<class_float>`\ )   |
   +---------------------------+---------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>`\ (\ from\: :ref:`String<class_String>`\ ) |
   +---------------------------+---------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>`\ (\ from\: :ref:`bool<class_bool>`\ )     |
   +---------------------------+---------------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>`\ (\ from\: :ref:`int<class_int>`\ )       |
   +---------------------------+---------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

Operators
---------

.. table::
   :widths: auto

   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator !=<class_float_operator_neq_float>`\ (\ right\: :ref:`float<class_float>`\ )               |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator !=<class_float_operator_neq_int>`\ (\ right\: :ref:`int<class_int>`\ )                     |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Color<class_Color>`           | :ref:`operator *<class_float_operator_mul_Color>`\ (\ right\: :ref:`Color<class_Color>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Quaternion<class_Quaternion>` | :ref:`operator *<class_float_operator_mul_Quaternion>`\ (\ right\: :ref:`Quaternion<class_Quaternion>`\ ) |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Vector2<class_Vector2>`       | :ref:`operator *<class_float_operator_mul_Vector2>`\ (\ right\: :ref:`Vector2<class_Vector2>`\ )          |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Vector2<class_Vector2>`       | :ref:`operator *<class_float_operator_mul_Vector2i>`\ (\ right\: :ref:`Vector2i<class_Vector2i>`\ )       |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`       | :ref:`operator *<class_float_operator_mul_Vector3>`\ (\ right\: :ref:`Vector3<class_Vector3>`\ )          |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`       | :ref:`operator *<class_float_operator_mul_Vector3i>`\ (\ right\: :ref:`Vector3i<class_Vector3i>`\ )       |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Vector4<class_Vector4>`       | :ref:`operator *<class_float_operator_mul_Vector4>`\ (\ right\: :ref:`Vector4<class_Vector4>`\ )          |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`Vector4<class_Vector4>`       | :ref:`operator *<class_float_operator_mul_Vector4i>`\ (\ right\: :ref:`Vector4i<class_Vector4i>`\ )       |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator *<class_float_operator_mul_float>`\ (\ right\: :ref:`float<class_float>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator *<class_float_operator_mul_int>`\ (\ right\: :ref:`int<class_int>`\ )                      |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator **<class_float_operator_pow_float>`\ (\ right\: :ref:`float<class_float>`\ )               |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator **<class_float_operator_pow_int>`\ (\ right\: :ref:`int<class_int>`\ )                     |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator +<class_float_operator_sum_float>`\ (\ right\: :ref:`float<class_float>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator +<class_float_operator_sum_int>`\ (\ right\: :ref:`int<class_int>`\ )                      |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator -<class_float_operator_dif_float>`\ (\ right\: :ref:`float<class_float>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator -<class_float_operator_dif_int>`\ (\ right\: :ref:`int<class_int>`\ )                      |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator /<class_float_operator_div_float>`\ (\ right\: :ref:`float<class_float>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator /<class_float_operator_div_int>`\ (\ right\: :ref:`int<class_int>`\ )                      |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator \<<class_float_operator_lt_float>`\ (\ right\: :ref:`float<class_float>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator \<<class_float_operator_lt_int>`\ (\ right\: :ref:`int<class_int>`\ )                      |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator \<=<class_float_operator_lte_float>`\ (\ right\: :ref:`float<class_float>`\ )              |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator \<=<class_float_operator_lte_int>`\ (\ right\: :ref:`int<class_int>`\ )                    |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator ==<class_float_operator_eq_float>`\ (\ right\: :ref:`float<class_float>`\ )                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator ==<class_float_operator_eq_int>`\ (\ right\: :ref:`int<class_int>`\ )                      |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator ><class_float_operator_gt_float>`\ (\ right\: :ref:`float<class_float>`\ )                 |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator ><class_float_operator_gt_int>`\ (\ right\: :ref:`int<class_int>`\ )                       |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator >=<class_float_operator_gte_float>`\ (\ right\: :ref:`float<class_float>`\ )               |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`             | :ref:`operator >=<class_float_operator_gte_int>`\ (\ right\: :ref:`int<class_int>`\ )                     |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator unary+<class_float_operator_unplus>`\ (\ )                                                 |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`           | :ref:`operator unary-<class_float_operator_unminus>`\ (\ )                                                |
   +-------------------------------------+-----------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Constructor Descriptions
------------------------

.. _class_float_constructor_float:

.. rst-class:: classref-constructor

:ref:`float<class_float>` **float**\ (\ ) :ref:`🔗<class_float_constructor_float>`

Constructs a default-initialized **float** set to ``0.0``.

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`float<class_float>` **float**\ (\ from\: :ref:`float<class_float>`\ )

Constructs a **float** as a copy of the given **float**.

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`float<class_float>` **float**\ (\ from\: :ref:`String<class_String>`\ )

Converts a :ref:`String<class_String>` to a **float**, following the same rules as :ref:`String.to_float()<class_String_method_to_float>`.

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`float<class_float>` **float**\ (\ from\: :ref:`bool<class_bool>`\ )

Cast a :ref:`bool<class_bool>` value to a floating-point value, ``float(true)`` will be equal to 1.0 and ``float(false)`` will be equal to 0.0.

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`float<class_float>` **float**\ (\ from\: :ref:`int<class_int>`\ )

Cast an :ref:`int<class_int>` value to a floating-point value, ``float(1)`` will be equal to ``1.0``.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Operator Descriptions
---------------------

.. _class_float_operator_neq_float:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator !=**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_neq_float>`

Returns ``true`` if two floats are different from each other.

\ **Note:** :ref:`@GDScript.NAN<class_@GDScript_constant_NAN>` doesn't behave the same as other numbers. Therefore, the results from this operator may not be accurate if NaNs are included.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_neq_int:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator !=**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_neq_int>`

Returns ``true`` if the integer has different value than the float.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Color:

.. rst-class:: classref-operator

:ref:`Color<class_Color>` **operator ***\ (\ right\: :ref:`Color<class_Color>`\ ) :ref:`🔗<class_float_operator_mul_Color>`

Multiplies each component of the :ref:`Color<class_Color>`, including the alpha, by the given **float**.

::

    print(1.5 * Color(0.5, 0.5, 0.5)) # Prints (0.75, 0.75, 0.75, 1.5)

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Quaternion:

.. rst-class:: classref-operator

:ref:`Quaternion<class_Quaternion>` **operator ***\ (\ right\: :ref:`Quaternion<class_Quaternion>`\ ) :ref:`🔗<class_float_operator_mul_Quaternion>`

Multiplies each component of the :ref:`Quaternion<class_Quaternion>` by the given **float**. This operation is not meaningful on its own, but it can be used as a part of a larger expression.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Vector2:

.. rst-class:: classref-operator

:ref:`Vector2<class_Vector2>` **operator ***\ (\ right\: :ref:`Vector2<class_Vector2>`\ ) :ref:`🔗<class_float_operator_mul_Vector2>`

Multiplies each component of the :ref:`Vector2<class_Vector2>` by the given **float**.

::

    print(2.5 * Vector2(1, 3)) # Prints (2.5, 7.5)

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Vector2i:

.. rst-class:: classref-operator

:ref:`Vector2<class_Vector2>` **operator ***\ (\ right\: :ref:`Vector2i<class_Vector2i>`\ ) :ref:`🔗<class_float_operator_mul_Vector2i>`

Multiplies each component of the :ref:`Vector2i<class_Vector2i>` by the given **float**. Returns a :ref:`Vector2<class_Vector2>`.

::

    print(0.9 * Vector2i(10, 15)) # Prints (9.0, 13.5)

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Vector3:

.. rst-class:: classref-operator

:ref:`Vector3<class_Vector3>` **operator ***\ (\ right\: :ref:`Vector3<class_Vector3>`\ ) :ref:`🔗<class_float_operator_mul_Vector3>`

Multiplies each component of the :ref:`Vector3<class_Vector3>` by the given **float**.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Vector3i:

.. rst-class:: classref-operator

:ref:`Vector3<class_Vector3>` **operator ***\ (\ right\: :ref:`Vector3i<class_Vector3i>`\ ) :ref:`🔗<class_float_operator_mul_Vector3i>`

Multiplies each component of the :ref:`Vector3i<class_Vector3i>` by the given **float**. Returns a :ref:`Vector3<class_Vector3>`.

::

    print(0.9 * Vector3i(10, 15, 20)) # Prints (9.0, 13.5, 18.0)

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Vector4:

.. rst-class:: classref-operator

:ref:`Vector4<class_Vector4>` **operator ***\ (\ right\: :ref:`Vector4<class_Vector4>`\ ) :ref:`🔗<class_float_operator_mul_Vector4>`

Multiplies each component of the :ref:`Vector4<class_Vector4>` by the given **float**.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_Vector4i:

.. rst-class:: classref-operator

:ref:`Vector4<class_Vector4>` **operator ***\ (\ right\: :ref:`Vector4i<class_Vector4i>`\ ) :ref:`🔗<class_float_operator_mul_Vector4i>`

Multiplies each component of the :ref:`Vector4i<class_Vector4i>` by the given **float**. Returns a :ref:`Vector4<class_Vector4>`.

::

    print(0.9 * Vector4i(10, 15, 20, -10)) # Prints (9.0, 13.5, 18.0, -9.0)

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_float:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator ***\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_mul_float>`

Multiplies two **float**\ s.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_mul_int:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator ***\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_mul_int>`

Multiplies a **float** and an :ref:`int<class_int>`. The result is a **float**.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_pow_float:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator ****\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_pow_float>`

Raises a **float** to a power of a **float**.

::

    print(39.0625**0.25) # 2.5

.. rst-class:: classref-item-separator

----

.. _class_float_operator_pow_int:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator ****\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_pow_int>`

Raises a **float** to a power of an :ref:`int<class_int>`. The result is a **float**.

::

    print(0.9**3) # 0.729

.. rst-class:: classref-item-separator

----

.. _class_float_operator_sum_float:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator +**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_sum_float>`

Adds two floats.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_sum_int:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator +**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_sum_int>`

Adds a **float** and an :ref:`int<class_int>`. The result is a **float**.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_dif_float:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator -**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_dif_float>`

Subtracts a float from a float.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_dif_int:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator -**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_dif_int>`

Subtracts an :ref:`int<class_int>` from a **float**. The result is a **float**.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_div_float:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator /**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_div_float>`

Divides two floats.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_div_int:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator /**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_div_int>`

Divides a **float** by an :ref:`int<class_int>`. The result is a **float**.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_lt_float:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator <**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_lt_float>`

Returns ``true`` if the left float is less than the right one.

\ **Note:** :ref:`@GDScript.NAN<class_@GDScript_constant_NAN>` doesn't behave the same as other numbers. Therefore, the results from this operator may not be accurate if NaNs are included.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_lt_int:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator <**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_lt_int>`

Returns ``true`` if this **float** is less than the given :ref:`int<class_int>`.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_lte_float:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator <=**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_lte_float>`

Returns ``true`` if the left float is less than or equal to the right one.

\ **Note:** :ref:`@GDScript.NAN<class_@GDScript_constant_NAN>` doesn't behave the same as other numbers. Therefore, the results from this operator may not be accurate if NaNs are included.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_lte_int:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator <=**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_lte_int>`

Returns ``true`` if this **float** is less than or equal to the given :ref:`int<class_int>`.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_eq_float:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator ==**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_eq_float>`

Returns ``true`` if both floats are exactly equal.

\ **Note:** Due to floating-point precision errors, consider using :ref:`@GlobalScope.is_equal_approx()<class_@GlobalScope_method_is_equal_approx>` or :ref:`@GlobalScope.is_zero_approx()<class_@GlobalScope_method_is_zero_approx>` instead, which are more reliable.

\ **Note:** :ref:`@GDScript.NAN<class_@GDScript_constant_NAN>` doesn't behave the same as other numbers. Therefore, the results from this operator may not be accurate if NaNs are included.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_eq_int:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator ==**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_eq_int>`

Returns ``true`` if the **float** and the given :ref:`int<class_int>` are equal.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_gt_float:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator >**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_gt_float>`

Returns ``true`` if the left float is greater than the right one.

\ **Note:** :ref:`@GDScript.NAN<class_@GDScript_constant_NAN>` doesn't behave the same as other numbers. Therefore, the results from this operator may not be accurate if NaNs are included.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_gt_int:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator >**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_gt_int>`

Returns ``true`` if this **float** is greater than the given :ref:`int<class_int>`.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_gte_float:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator >=**\ (\ right\: :ref:`float<class_float>`\ ) :ref:`🔗<class_float_operator_gte_float>`

Returns ``true`` if the left float is greater than or equal to the right one.

\ **Note:** :ref:`@GDScript.NAN<class_@GDScript_constant_NAN>` doesn't behave the same as other numbers. Therefore, the results from this operator may not be accurate if NaNs are included.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_gte_int:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator >=**\ (\ right\: :ref:`int<class_int>`\ ) :ref:`🔗<class_float_operator_gte_int>`

Returns ``true`` if this **float** is greater than or equal to the given :ref:`int<class_int>`.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_unplus:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator unary+**\ (\ ) :ref:`🔗<class_float_operator_unplus>`

Returns the same value as if the ``+`` was not there. Unary ``+`` does nothing, but sometimes it can make your code more readable.

.. rst-class:: classref-item-separator

----

.. _class_float_operator_unminus:

.. rst-class:: classref-operator

:ref:`float<class_float>` **operator unary-**\ (\ ) :ref:`🔗<class_float_operator_unminus>`

Returns the negative value of the **float**. If positive, turns the number negative. If negative, turns the number positive. With floats, the number zero can be either positive or negative.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
