---
title: "Write Frequency Matrix Element"
weight: 1000
---

# Write Frequency Matrix Element

This element saves all input frequency matrices to a specified location.

**Element type:** fmatrix-write

## Parameters

| Parameter        | Description                                                                                                                                   | Default Value | Parameter in Workflow File | Type     |
|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Output file** (required) | Location of the output data file. If this is set, the "Location" slot is not taken into account.                                      |               | url-out                    | _string_ |
| **Existing file**          | If a target file already exists, specify how it should be handled: overwritten, renamed, or appended (if supported by the file format). | Rename        | write-mode                 | _numeric_|

Available values for **Existing file** are:

- 0 - Overwrite
- 1 - Append
- 2 - Rename

## Input/Output Ports

The element has one _input port_:

**Name in GUI:** _Frequency matrix_

**Name in Workflow File:** in-fmatrix

**Slots:**

| Slot In GUI       | Slot in Workflow File | Type       |
|-------------------|-----------------------|------------|
| **Frequency matrix** | **fmatrix**           | _fmatrix_  |
| **Source URL**       | **url**               | _string_   |