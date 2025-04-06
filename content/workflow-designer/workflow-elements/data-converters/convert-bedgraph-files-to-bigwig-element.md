---
title: "Convert bedGraph Files to bigWig Element"
weight: 1
---


# Convert bedGraph Files to bigWig Element

Convert bedGraph files to bigWig.

**Element type:** bgtbw-bam

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

**Genome**

File with genome length.

human.hg18

**genome**

_string_

**Output name**

A name of an output file. If default of empty value is provided the output name is the name of the first file with additional extention.



**out-name**

_string_

**Block size**

Number of items to bundle in r-tree (-blockSize).

256

**bs**

_numeric_

**Items per slot**

Number of data points bundled at lowest level (-itemsPerSlot).

1024

**its**

_numeric_

**Uncompressed**

If set, do not use compression.(-unc).

False

**unc**

_boolean_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** BedGrapgh files

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_

And 1 _output port_:

**Name in GUI:** BigWig files

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
