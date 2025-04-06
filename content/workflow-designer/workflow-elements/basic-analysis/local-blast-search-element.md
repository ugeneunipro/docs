---
title: "Local BLAST Search Element"
weight: 1
---


# Local BLAST Search Element

Finds annotations for DNA sequence in a local BLAST database.

**Element type:** blast-plus



BLAST+ is used as an external tool from UGENE and it must be installed on your system. To learn more about the external tools, please, read main [UGENE User Manual](http://ugene.unipro.ru/documentation.html).

Parameters



Parameter

Description

Default value

Parameter in Workflow File

Type

**Search type**

Selects the type of the BLAST searches.

blastn

**blast-type**

_string_

Available values are:

*   blastn
*   blastp
*   blastx
*   tblastn
*   tblastx

**Database path**

Path to the database files.



**db-path**

_string_

**Database name**

Base name for BLAST DB files.



**db-name**

_string_

**Tool path**

Path to the BLAST executable.

default

**tool-path**

_string_

**Temporary directory**

Directory for temporary files.

default

**temp-dir**

_string_

**Expected value**

Expectation threshold value.

10

**e-val**

_numeric_

**Culling limit**

If the query range of a hit is enveloped by that of at least this many higher-scoring hits, delete the hit

0

**max-hits**

_numeric_

**Annotate as**

Name of the result annotations.

blast\_result

**result-name**

_string_

**Gapped alignment**

Perform gapped alignment.

use

**gapped-aln**

_boolean_

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

**BLAST output**

Location of BLAST output file.



**blast-output**

_string_

**BLAST output type**

Type of BLAST output file.

XML (-outfmt 5)

**type-output**

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
