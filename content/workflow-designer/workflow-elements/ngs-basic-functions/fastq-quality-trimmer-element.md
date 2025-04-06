---
title: "FASTQ Quality Trimmer Element"
weight: 1
---


# FASTQ Quality Trimmer Element

The workflow scans each input sequence from the end to find the first position where the quality is greater or equal to the minimum quality threshold. Then it trims the sequence to that position. If a the whole sequence has quality less than the threshold or the length of the output sequence less than the minimum length threshold then the sequence is skipped.

**Element type:** QualityTrim

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

**Output file name**

A name of an output file. If default of empty value is provided the output name is the name of the first file with additional extention.



**out-name**

_string_

**Quality threshold**

Quality threshold for trimming.

30

**qual-id**

_numeric_

**Min Length**

Too short reads are discarded by the filter.

0

**len-id**

_numeric_

**Trim both ends**

Trim the both ends of a read or not. Usually, you need to set True for Sanger sequencing and False for NGS

True

**both-ends**

_boolean_

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

And 1 _output port_:

**Name in GUI:** Output File

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
