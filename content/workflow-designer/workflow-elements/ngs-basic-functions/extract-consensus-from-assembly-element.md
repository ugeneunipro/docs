---
title: "Extract Consensus from Assembly Element"
weight: 300
---


# Extract Consensus from Assembly Element

Extract the consensus sequence from the incoming assembly.

**Element type:** extract-consensus

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Algorithm**

The algorithm of consensus extracting.

Default

**algorithm**

_string_

**Keep gaps**

Set this parameter if the result consensus must keep the gaps.

True

**keep-gaps**

_boolean_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** in-assembly

**Name in Workflow File:** in-assembly

**Slots:**



Slot In GUI

Slot in Workflow File

Type

**Assembly data**

**assembly**

_assembly_

And 1 _outut port_:

**Name in GUI:** out-sequence

**Name in Workflow File:** out-sequence

**Slots:**



Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_string_
