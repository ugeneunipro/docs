---
title: "Write NGS Reads Assembly Element"
weight: 1
---


# Write NGS Reads Assembly Element

The element gets message(s) with assembled reads data and saves the data to the specified file(s) in one of the appropriate formats (SAM, BAM, or UGENEDB).

**Element type:** write-assembly

Parameters



Parameter

Description

Default value

Parameter in Workflow File

Type

**Data storage**

Place to store workflow results: local file system or a database.



**data-storage**

_string_

**Document format**

Document format of the output file.

bam

**document-format**

_string_

**Build index (BAM only)**

Build BAM index for the target BAM file. The file .bai will be created in the same directory.

True

**build-index**

_boolean_

**Output file**

Location of output data file. If this attribute is set, slot "Location" in port will not be used.



**out-url**

_string_

**Output file suffix**

This suffix will be used for generating the output file name.



**url-suffix**

_string_

**Existing file**

If a target file already exists, you can specify how it should be handled: either overwritten, renamed or appended (if supported by file format). If Rename option is chosen existing file will be renamed.

Rename

**write-mode**

_numeric_



Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** _Assembly_

**Name in Workflow File:** in-assembly

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Assembly data**

**assembly**

_assembly_

**Location**

**url**

_string_
