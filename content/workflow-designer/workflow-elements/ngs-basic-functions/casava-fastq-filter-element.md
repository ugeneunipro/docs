---
title: "CASAVA FASTQ Filter Element"
weight: 100
---


# CASAVA FASTQ Filter Element

Reads in FASTQ file produced by CASAVA 1.8 contain 'N' or 'Y' as a part of an idetifier. 'Y' if a read if filtered, 'N' if the read if the read is not filtered. The workflow cleans up the filtered reads. For example: @HWI-ST880:181:D1WRUACXX:8:1102:4905:2125 1:N:0:TAAGGG CTTACATAACTACTGACCATGCTCTCTCTTGTCTGTCTCTTATACACATCT + 111442222322324232AAFFHIJJJJJJIHIIF111CGGFHIG???FGB @HWI-ST880:181:D1WRUACXX:8:1102:7303:2101 1:Y:0:TAAGGG TCCTTACTGTCTGAGCAATGGGATTCCATCTTTTACGATCTAGACATGGCT + 11++4222322.

**Element type:** CASAVAFilter

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

Input/Output Ports

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
