---
title: "Align with MUSCLE Element"
weight: 1
---


# Align with MUSCLE Element

MUSCLE is public domain multiple alignment software for protein and nucleotide sequences. MUSCLE stands for MUltiple Sequence Comparison by Log-Expectation.

**Element type:** muscle

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Mode**

Selector of preset configurations, that give you the choice of optimizing accuracy, speed, or some compromise between the two. The default favors accuracy.

MUSCLE default

**mode**

_numeric_

Availables values are:

*   0 - for MUSCLE default
*   1 - for Large alignment
*   2 - for Refine only

**Stable order**

Do not rearrange aligned sequences (-stable switch of MUSCLE). Otherwise, MUSCLE re-arranges sequences so that similar sequences are adjacent in the output file. This makes the alignment easier to evaluate by eye.

True

**stable**

_boolean_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input MSA_

**Name in Workflow File:** in-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_

And 1 _output port_:

**Name in GUI:** _Multiple sequence alignment_

**Name in Workflow File:** out-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_
