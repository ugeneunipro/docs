---
title: "Write Weight Matrix Element"
weight: 1200
---

# Write Weight Matrix Element

This function saves all input weight matrices to a specified location.

**Element type:** wmatrix-write

Parameters
----------

| Parameter       | Description                                                                                                                         | Default value | Parameter in Workflow File | Type     |
|-----------------|-------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Output file** | Location of the output data file. If this attribute is set, the “Location” slot is not taken into account.                           |               | url-out                    | _string_ |
| **Existing file** | If a target file already exists, you can specify how it should be handled: either overwritten, renamed, or appended (if supported by the file format). | Rename        | write-mode                 | _numeric_ |

Available values for "Existing file" are:

* 0 - for overwrite
* 1 - for append
* 2 - for rename

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** _Weight matrix_

**Name in Workflow File:** in-wmatrix

**Slots:**

| Slot In GUI      | Slot in Workflow File | Type      |
|------------------|-----------------------|-----------|
| **Weight matrix** | wmatrix               | _wmatrix_ |
| **Source URL**   | url                   | _string_  |