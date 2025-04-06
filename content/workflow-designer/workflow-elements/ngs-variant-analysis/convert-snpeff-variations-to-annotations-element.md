---
title: "Convert SnpEff Variations to Annotations Element"
weight: 1
---


# Convert SnpEff Variations to Annotations Element

Parses information, added to variations by SnpEff, into standard annotations.

**Element type:** convert-snpeff-variations-to-annotations

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output file**

Location of output data file. If this attribute is set, slot "Location" in port will not be used.



url-out

_string_

**Document format**

Document format of the output file.

 genbank

document-format

_string_

Input/Output Ports

The element has 1 _input ports_:

**Name in GUI:** Input file URL

**Name in Workflow File:** in-variations-url

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
