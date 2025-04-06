---
title: "Remote BLAST Element"
weight: 1
---


# Remote BLAST Element

Finds annotations for the supplied DNA sequence in the NCBI remote database.

Element type: **blast**

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Database**

Selects the database to search through. Available databases are blastn, blastp and cdd.

ncbi-blastn

**db**

_string_

Available values are:

*   ncbi-blastn
*   ncbi-blastp
*   ncbi-cdd

**Database**

Select the database to search through.



**db**

_string_

**Expected value**

This parameter specifies the statistical significance threshold of reporting matches against the database sequences.

10

**e-val**

_string_

**Results limit**

The maximum number of results.

10

**hits**

_numeric_

**Megablast**

Use megablast.

False

**megablast**

_boolean_

**Short sequence**

Optimizes search for short sequences.

False

**short-sequence**

_boolean_

**Entrez query**

Enter an Entrez query to limit search.



**entrez-query**

_string_

**Annotate as**

Name of the result annotations.



**result-name**

_string_

**BLAST output**

Location of the BLAST output file. This parameter insignificant for cdd search.



**blast-output**

_string_

**Gap costs**

Cost to create and extend a gap in an alignment.

2 2

**gap-costs**

_string_

**Match scores**

Reward and penalty for matching and mismatching bases.

1 -3

**match-scores**

_string_



Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input sequence_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

And 1 _output port_:

**Name in GUI:** _Annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
