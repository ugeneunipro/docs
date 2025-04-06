---
title: "Sequence Quality Trimmer Element"
weight: 1
---


# Sequence Quality Trimmer Element

Scans each input sequence from the end to find the first position where the quality is greater or equal to the minimum quality threshold.

Then it trims the sequence to that position.

If a whole sequence has quality less than the threshold or the length of the output sequence less than the minimum length threshold then the sequence is skipped.

**Elemet type:** SequenceQualityTrim

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Trimming quality threshold**

Quality threshold for trimming.

30

**qual-id**

_numeric_

**Min length**

Too short reads are discarded by the filter.

0

**len-id**

_numeric_

**Trim both ends**

Trim both ends of a read or not. Usually, you need to set **True** for **Sanger** sequencing and **False** for **NGS**

True

**both-ends**

_boolean_

Input/Output Ports
------------------

The element has 1 _input port._

**Name in GUI:** _Input data_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

 And 1 _output port_:

**Name in GUI:** _Output data_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

__sequence__
