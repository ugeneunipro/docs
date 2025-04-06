---
title: "Amino Acid Translation Element"
weight: 1
---


# Amino Acid Translation Element

Translates a sequence into its amino translation or translations.

**Element type:** sequence-translation

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Translate from**

Specifies position that should be used to translate the sequence from: first, second, third or all (three output amino sequences would be generated).

all

**pos-2-translate**

_string_

Available values are:

*   all
*   first
*   second
*   third

**Auto selected genetic code**

Specifies that genetic code should be selected automatically.

True

**auto-translation**

_boolean_

**Genetic code**

Genetic code that should be used to translate the input nucleotide sequence.

The Standard Genetic Code

**genetic-code**

_string_



Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input Data_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

And 1 _output port_:

**Name in GUI:** _Amino sequence_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

**Plain text**

**text**

_string_
