---
title: "Write HMM3 Profile"
weight: 400
---


# Write HMM3 Profile

Saves all input HMM3 profiles to the specified locations.

**Element type:** hmm3-write-profile

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output file**

Location of the output data file. If this attribute is set, the “Location” slot is not taken into account.



**url-out**

_string_

**Existing file**

If a target file already exists, you can specify how it should be handled: either overwritten, renamed or appended (if supported by file format). If Rename option is chosen existing file will be renamed.

Rename

**write-mode**

_numeric_

Available values are:

*   0 - for overwrite
*   1 - for append
*   2 - for rename

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** _HMM3 profile_

**Name in Workflow File:** in-hmm3

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**HMM profile**

**hmm3-profile**

_hmm3-profile_

**Location**

**url**

_string_
