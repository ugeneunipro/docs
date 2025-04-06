---
title: "Extract Transcript Sequences with gffread Element"
weight: 1
---


# Extract Transcript Sequences with gffread Element

Extract transcript sequences from the genomic sequence(s) with gffread.

**Element type:** gffread

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output sequences**

The url to the output file with the extracted sequences.



**url-out**

_string_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input transcripts

**Name in  Workflow File:** in-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Genomic sequence url**

**genome**

__string__

**Transcripts url**

**transcripts**

_string_

And 1 _output port_:

**Name in GUI:** Extracted sequences url

**Name in Workflow File:** extracted-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**sequences**

**sequences**

__string__
