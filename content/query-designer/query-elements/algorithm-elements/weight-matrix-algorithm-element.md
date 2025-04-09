---
title: "Weight Matrix Algorithm Element"
weight: 1300
---


# Weight Matrix Algorithm Element

The _element_ searches the input sequence for transcription factor binding sites (TFBSs) significantly similar to the specified weight matrix.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Annotate As**

Name of the result annotations.

misc\_feature

**Direction**

See the description [_here_](../../manipulating-schema/managing-strands/element-direction-in-schema).

Any

**Matrix**

Path to the profile.

You must specify a value!

**Min score**

Minimum score to detect TFBS.

85%

Parameters in Schema File
-------------------------

**Type:** wsearch

Parameter

Parameter in the GUI

Type

**key**

**Annotate As**

_string_

**matrix**

**Matrix**

_string_

**min-score**

**Min score**

_numeric_

**strand**

**Direction**

_string_

Available values are:

*   complement
*   direct
*   both
