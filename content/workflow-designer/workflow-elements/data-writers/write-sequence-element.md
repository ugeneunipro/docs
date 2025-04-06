---
title: "Write Sequence Element"
weight: 1
---


# Write Sequence Element

The element gets message(s) with sequence data and, optionally, associated annotations data and saves the data to the specified file(s) in one of the appropriate formats (GenBank, FASTA, etc.).

**Element type:** write-sequence

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Data storage**

Place to store workflow results: local file system or a database.



**data-storage**

_string_

**Output file**

Location of the output data file. If this attribute is set, then the “Location” slot is not taken into account.



**url-out**

_string_

**Output file suffix**

This suffix will be used for generating the output file name.



**url-suffix**

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

**Document format**

Format of the output file.

fasta

**document-format**

_string_

Available values are:

*   fasta
*   fastq
*   genbank
*   raw

**Accumulate objects**

Accumulates all incoming data in one file or creates separate files for each input. In the latter case, an incremental numerical suffix is added to a file name.

True

**accumulate**

_boolean_

**Split sequence**

Split each incoming sequence on several parts.

1

**split**

_numeric_



Input/Output Ports
------------------

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

**Set of annotations**

**annotations**

_annotation-table-list_
