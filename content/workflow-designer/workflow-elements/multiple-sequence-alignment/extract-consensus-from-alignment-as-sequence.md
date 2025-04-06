---
title: "Extract Consensus from Alignment as Sequence"
weight: 1
---


# Extract Consensus from Alignment as Sequence

Extract the consensus sequence from the incoming multiple sequence alignment.

**Element type:** extract-msa-consensus-sequence

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Algorithm**

The algorithm of consensus extracting.



**algorithm**

_string_

**Threshold**

The threshold of the algorithm.

100

**threshold**

_numeric_

**Keep gaps**

Set this parameter if the result consensus must keep the gaps.

True

**keep-gaps**

_boolean_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** _in-msa_

**Name in Workflow File:** in-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_

And 1 _output port_:

**Name in GUI:** _out-sequence_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_seq_
