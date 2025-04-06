---
title: "Get Sequences by Annotations Element"
weight: 1
---


# Get Sequences by Annotations Element

Extracts annotated regions from the input sequence.

**Element type:** extract-annotated-sequence

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Translate**

Translates the annotated regions if the corresponding annotation marks a protein subsequence.

False

**translate**

_boolean_

**Complement**

Complements the annotated regions if the corresponding annotation is located on the complement strand.

False

**complement**

_boolean_

**Split joined**

Split joined annotations to single region annotations.

False

**split-joined-annotations**

_boolean_

**Extend left**

Extends the resulted regions to left.

0

**extend-left**

_numeric_

**Extend right**

Extends the resulted regions to right.

0

**extend-right**

_numeric_

**Gap length**

Inserts a gap of a specified length between the merged locations of the annotation.

0

**merge-gap-length**

_numeric_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input sequence_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

**Set of annotations**

**annotations**

_annotation-table_

And 1 _output port_:

**Name in GUI:** _Annotated regions_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_
