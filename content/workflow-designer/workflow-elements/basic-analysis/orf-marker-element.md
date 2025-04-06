---
title: "ORF Marker Element"
weight: 1
---


# ORF Marker Element

Finds Open Reading Frames (ORFs) in each supplied nucleotide sequence, stores found regions as annotations.

**Element type:** orf-search

Parameters in GUI
-----------------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Annotate as** (required)

Name of the result annotations.

ORF

**result-name**

_string_

**Search in**

Specifies which strands should be searched: direct, complement or both.

both strands

**strand**

_numeric_

Available values are:

*   0 - for searching in both strands
*   1 - for searching in direct strand
*   2 - for searching in complement strand

**Min length**

Ignores ORFs shorter than the specified length.

100

**min-length**

_numeric_

**Genetic code**

Specifies which genetic code should be used for translating the input nucleotide sequence.

The Standard Genetic Code

**genetic-code**

_string_

Available values are:

*   NCBI-GenBank #1
*   NCBI-GenBank #2
*   etc.

**Require init codon**

Allows or not ORFs starting with any codon other than terminator.

True

**require-init-codon**

_boolean_

**Require stop codon**

Ignores boundary ORFs which last beyound the search region (i.e. have no stop codon within the range).

False

**require-stop-codon**

_boolean_

**Allow alternative codons**

Allows ORFs starting with alternative initiation codons, accordingly to the current translation table.

False

**allow-alternative-codons**

_boolean_

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

**Name in GUI:** _ORF annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
