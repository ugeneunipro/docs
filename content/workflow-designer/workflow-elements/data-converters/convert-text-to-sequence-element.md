---
title: "Convert Text to Sequence Element"
weight: 200
---


# Convert Text to Sequence Element

Converts the input text to a sequence.

**Element type:** convert-text-to-sequence

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Sequence name** (required)

Result sequence name.

_Sequence_

**sequence-name**

_string_

**Sequence alphabet**

Alphabet of the sequence. Chooose _Auto_ to auto-detect the alphabet or one of the following values:

*   _All symbols_
*   _Extended DNA_
*   _Extended RNA_
*   _Standard DNA_
*   _Standard RNA_
*   _Standard amino_

_Auto_

**alphabet**

_string_

**Skip unknown symbols**

If _True_, ignores all symbols that are not presented in the sequence alphabet selected.

_True_

**skip-unknown**

_boolean_

**Replace unknown symbols with**

Replaces all unknown symbols with the specified symbol.

_N_

**replace-unknown-with**

_string_

(1 character)

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input text_

**Name in Workflow File:** in-text

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Plain text**

**text**

_string_

And 1 _output port_:

**Name in GUI:** _Output sequence_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_
