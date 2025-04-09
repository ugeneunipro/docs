---
title: "Fetch Sequences by ID From Annotation Element"
weight: 600
---


# Fetch Sequences by ID From Annotation Element

Parses annotations to find any IDs and fetches corresponding sequences.

**Element type:** fetch-sequence

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Save file to directory**

The directory to store sequence files loaded from a database.

default

**save-dir**

_string_

**NCBI database**

The database to read from.

nucleotide

Available values are:

*   nucleotide
*   protein

**database**

_string_



Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** _Input annotations_

**Name in Workflow File:** in-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_

And 1 _output port_:

**Name in GUI:** _Sequence_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_

**Sequence**

**sequence**

_sequence_
