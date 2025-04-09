---
title: "FastQC Quality Control Element"
weight: 700
---


# FastQC Quality Control Element

Builds quality control reports.

**Element type:** fastqc

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output file**

Specify the output file name.

Input file

**out-file**

_string_

**List of adapters**

Specifies a non-default file which contains the list of adapter sequences which will be explicity searched against the library. The file must contain sets of named adapters in the form name\[tab\]sequence. Lines prefixed with a hash will be ignored.



**adapter**

_string_

**List of contaminants**

Specifies a non-default file which contains the list of contaminants to screen overrepresented sequences against. The file must contain sets of named contaminants in the form name\[tab\]sequence. Lines prefixed with a hash will be ignored.



**contaminants**

_string_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Short reads

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
