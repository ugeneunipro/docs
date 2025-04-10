---
title: "Write SITECON Model Element"
weight: 1100
---

# Write SITECON Model Element

Saves all input SITECON profiles to a specified location.

**Type:** sitecon-write

Parameters
----------

| Parameter       | Description                                                                                                                                                                  | Default value | Parameter in Workflow File | Type          |
|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|---------------|
| **Output file** | Location of the output data file. If this attribute is set, the “Location” slot is not considered.                                                                           |               | **url-out**                | _string_      |
| **Existing file** | If a target file already exists, you can specify how it should be handled: either overwritten, renamed, or appended (if supported by the file format).                       | Rename        | **write-mode**             | _numeric_     |

Available values for **Existing file** are:

*   0 - for overwrite
*   1 - for append
*   2 - for rename

Input/Output Ports

The element has 1 _input port_:

| Slot In GUI       | Slot in Workflow File | Type            |
|-------------------|-----------------------|-----------------|
| **Sitecon model** | sitecon-model         | _sitecon-model_ |
| **Source URL**    | url                    | _string_        |

**Name in GUI:** _Sitecon model_

**Name in Workflow File:** in-sitecon