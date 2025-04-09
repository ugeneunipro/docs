---
title: "Merge BAM Files Element"
weight: 1100
---


# Merge BAM Files Element

Merge BAM files using SAMTools merge.

**Element type:** merge-bam

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.



**out-mode**

_numeric_

**Custom directory**

Custom output directory.



**custom-dir**

_string_

**Output BAM name**

A name of an output BAM file. If default of empty value is provided the output name is the name of the first BAM file with .merged.bam extention.



**out-name**

_string_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** BAM File

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**input-url**

_string_

And 1 _out__put port_:

**Name in GUI:** Merged BAM files

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**output-url**

_string_
