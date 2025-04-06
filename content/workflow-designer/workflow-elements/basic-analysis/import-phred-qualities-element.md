---
title: "Import PHRED Qualities Element"
weight: 1
---


# Import PHRED Qualities Element

Adds corresponding PHRED quality scores to the sequences. Use this element to convert .fasta and .qual pair to fastq format.

**Element type:** import-phred-qualities

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**PHRED input** (required)

Path to a file with PHRED quality scores.



**url-in**

_string_

**Quality format**

Format to encode quality scores.

Sanger

**quality-format**

_string_

Available values are:

*   Sanger
*   Illumina 1.3+
*   Solexa/Illumina 1.0

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _DNA sequences_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

And 1 _output port_:

**Name in GUI:** _DNA sequences with imported quailities_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_
