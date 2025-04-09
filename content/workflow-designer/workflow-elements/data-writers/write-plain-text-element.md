---
title: "Write Plain Text Element"
weight: 500
---


# Write Plain Text Element

The element gets message(s) with text data and saved the data to the specified text file(s).

**Element type:** write-text

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

**Output file**

Location of the output data file. If this attribute is set, then the “Location” slot is not taken into account.



**url-out**

_string_

**Output file suffix**

This suffix will be used for generating the output file name.



**url-suffix**

_string_

**Existing file**

If a target file already exists, you can specify how it should be handled: either overwritten, renamed or appended (if supported by file format).

Rename

**write-mode**

_numeric_

Available values are:

*   0 - for overwrite
*   1 - for append
*   2 - for rename

**Accumulate objects**

Accumulates all incoming data in one file or creates separate files for each input. In the latter case, an incremental numerical suffix is added to a file name.

True

**accumulate**

_boolean_



Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Plain text_

**Name in Workflow File:** in-text

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Plain text**

**text**

_string_

**Location**

**url**

_string_
