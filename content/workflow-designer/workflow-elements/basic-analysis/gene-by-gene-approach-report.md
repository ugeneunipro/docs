---
title: "Gene-by-gene approach report"
weight: 1200
---


# Gene-by-gene approach report

Output a table of genes found in a reference sequence.

**Element type:** genebygene-report-id

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output file**

File to store a report.



**output-file**

_string_

**Annotation name**

Annotation name used to compare genes and reference genomes.

blast-result

**annotation\_name**

_string_

**Existing file**

If a target report already exists you should specify how to handle that. Merge two table in one. Overwrite or Rename existing file.

Merge

**existing**

_string_

**Identity cutoff**

Identity between gene sequence length and annotation length in percent. BLAST identity (if specified) is checked after

90.0000%

**identity**

_numeric_



Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Gene by gene report data

**Name in Workflow File:** in-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Input annotations**

**gene-ann**

_ann-table-list_

**Input sequences**

**gene-seq**

_seq_
