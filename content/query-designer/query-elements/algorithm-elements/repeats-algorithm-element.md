---
title: "Repeats Algorithm Element"
weight: 700
---


# Repeats Algorithm Element

The _element_ searches for repeats in the input sequence.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Annotate As**

Name of the result annotations.

repeat\_unit

**Algorithm**

Algorithm used to search for repeats. Available values are:

*   Suffix index
*   Diagonals
*   Auto

Suffix index

**Filter nested**

If _True_, filters nested repeats.

True

**Identity**

Repeats percentage identity.

100%

**Inverted**

If _True_, searches for inverted repeats.

False

**Min length**

Minimum length of repeats.

5bp

**Max length**

Maximum length of repeats.

10000bp

**Parallel threads**

Number of parallel threads used to execute the calculations.

Auto

Parameters in Schema File
-------------------------

**Type:** repeats

Parameter

Parameter in the GUI

Type

**key**

**Annotate As**

_string_

**algorithm**

**Algorithm**

_string_

Available values are:

*   suffix
*   diagonals
*   auto

**filter-nested**

**Filter nested**

_boolean_

**identity**

**Identity**

_numeric_

**invert**

**Invert**

_boolean_

**min-length**

**Min length**

_numeric_

**max-length**

**Max length**

_numeric_

**threads**

**Parallel threads**

_numeric_
