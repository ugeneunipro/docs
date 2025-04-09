---
title: "Tandem Repeats Algorithm Element"
weight: 1200
---


# Tandem Repeats Algorithm Element

The _Tandem repeats_ _element_ finds tandem repeats in a supplied sequence, stores found regions as annotations.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Annotate As**

Name of the result annotations.

repeate\_unit

**Direction**

See the description [_here_](element-direction-in-schema.md).

Any

**Algorithm**

The algorithm parameter allows one to select the search algorithm. The default and a fast one is the optimized suffix array algorithm.

Suffix index(optimized)

**Min period**

Minimum acceptable repeat length measured in base symbols.

1 n

**Max period**

Maximum acceptable repeat length measured in base symbols.

1000000 n

**Min tandem size**

The minimum tandem size sets the limit on minimum acceptable length of the tandem, i.e. the minimum total repeats length of the searched tandem.

9

**Min repeat count**

The minimum number of repeats of a searched tandem.

x3

**Search for overlapped tandems**

If this parameter is set to _True_ then overlapped tandems should be included into the result.



**Parallel threads**

Number of parallel threads used for the task.

Auto

Parameters in Schema File
-------------------------

**Type:** tandems

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

*   Suffix index
*   Suffix index (optimized)

**min-period**

**Min period**

_numeric_

**max-period**

**Max period**

_numeric_

**min-tandem-size**

**Min tandem size**

_numeric_

**min-repeat-count**

**Min repeat count**

_numeric_

**show-overlapped-tandems**

**Search for overlapped tandems**

_boolean_

**strand**

**Direction**

_string_

Available values are:

*   complement
*   direct
*   both

**n-threads**

**Parallel threads**

_string_
