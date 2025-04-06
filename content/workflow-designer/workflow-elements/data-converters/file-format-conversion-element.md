---
title: "File Format Conversion Element"
weight: 1
---


# File Format Conversion Element

Converts the file to the selected format if it is not excluded.

**Element type:** files-conversion

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Document format**

Document format of the output file.



**document-format**

_string_

**Excluded formats**

The input file won't be converted to any of the selected formats.



**excluded-formats**

_string_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** File

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**input-url**

_string_

And 1 _out__put port_:

**Name in GUI:** File

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**output-url**

_string_
