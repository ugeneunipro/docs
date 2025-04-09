---
title: "Read Sequence Element"
weight: 800
---


# Read Sequence Element

Input one or several files with nucleotide or protein sequences.

A file may also contain annotations. Any format, supported by UGENE, is allowed (GenBank, FASTA, etc.).

The element outputs message(s) with the sequence and annotations data.

See the list of all available formats [here](https://local.ugene.unipro.ru/wiki/display/UUOUM27/Appendix+A.+Supported+File+Formats).

**Element type:** read-sequence



Parameters in GUI
-----------------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Input files**

Semicolon-separated list of datasets to the input files.



**url-in**

_string_

**Mode**

If the file contains more than one sequence, “split” mode sends them as is to output, while “merge” appends all the sequences and outputs the merged sequence.

Split

**mode**

_numeric_

Available values are:

*   0 - for split mode
*   1 - for merge mode

**Merging gap**

In the “merge” mode, inserts the specified number of gaps between the original sequences. This is helpful e.g. to avoid finding false positives at the merge boundaries.

10

**merge-gap**

_numeric_

**Sequence count limit**

Split mode only. Read only first N sequences from each file. Set 0 value for reading all sequences.

0

**sequence-count-limit**

_numeric_

**Accession filter**

Only reports a sequence with the specified accession (id).



**accept-accession**

_string_



Input/Output Ports

The element has 1 _output port_:

**Name in GUI:** _Sequence_

**Name in Workflow File:** out-sequence

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

**Source URL**

**url**

_string_
