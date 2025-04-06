---
title: "Merge Annotations Element"
weight: 1
---


# Merge Annotations Element

Writes all supplied sequences to file(s) in FASTQ format.

**Element type:** write-fastq

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output file** (required)

Location of the output data file. If this attribute is set, then the “Location” slot is not taken into account.



**url-out**

_string_

**Existing file**

If a target file already exists, you can specify how it should be handled: either overwritten, renamed or appended (if supported by file format).

Rename

**write-mode**

_numeric_

Available values are:

*   0 - for overwrite
*   1 - for append
*   2 - for rename

**Accumulate objects**

Accumulates all incoming data in one file or creates separate files for each input. In the latter case, an incremental numerical suffix is added to a file name.

True

**accumulate**

_boolean_



Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Sequence_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

**Location**

**url**

_string_
