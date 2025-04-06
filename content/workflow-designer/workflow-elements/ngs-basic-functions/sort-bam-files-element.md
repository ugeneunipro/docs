---
title: "Sort BAM Files Element"
weight: 1
---


# Sort BAM Files Element

Sort BAM Files using SAMTools Sort.

**Element type:** Sort-bam

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.

Input file

**out-mode**

_numeric_

**Custom directory**

Specify the output directory.



**custom-dir**

_string_

**Output BAM name**

A name of an output file. If default of empty value is provided the output name is the name of the first file with additional extention.



**out-name**

_string_

**Build index**

Build index for the sorted file with SAMTools index.

human.hg18

**index**

_boolean_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** BAM File

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_

And 1 _output port_:

**Name in GUI:** Sorted BAM File

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
