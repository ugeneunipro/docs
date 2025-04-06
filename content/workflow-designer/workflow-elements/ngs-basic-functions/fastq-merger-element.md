---
title: "FASTQ Merger Element"
weight: 1
---


# FASTQ Merger Element

Merges input sequences to one output file.

**Element type:** MergeFastq

 Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.



**out-mode**

_string_

**Output file name**

A name of an output file. If default of empty value is provided the output name is the name of the first file with additional extention.



**out-name**

_string_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input File

**Name in Workflow File:** in-file

**Slots:**



Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_

The element has 1 _output port_:

**Name in GUI:** Output File

**Name in Workflow File:** out-file

**Slots:**



Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
