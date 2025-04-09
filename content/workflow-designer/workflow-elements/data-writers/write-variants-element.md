---
title: "Write Variants Element"
weight: 700
---


# Write Variants Element

The element gets message(s) with variations data and saves the data to the specified file(s) in one of the appropriate formats (e.g. VCF).

**Element type:** write-variations



Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Data storage**

Place to store workflow results: local file system or a database.



**data-storage**

_split_

**Accumulate objects**

Accumulate all incoming data in one file or create separate files for each input.In the latter case, an incremental numerical suffix is added to the file name.

True

**accumulate**

_boolean_

**Document format**

Document format of output file.

snp

**document-format**

_string_

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

**Name in GUI:** Variation track

**Name in Workflow File:** in-variations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Location**

**url**

_string_

**Variation track**

**variation-track**

_variation_
