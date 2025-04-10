---
title: "Write FASTA Element"
weight: 300
---

# Write FASTA Element

This element receives message(s) with sequence data and saves the data to the specified file(s) in FASTA format.

**Element type:** write-fasta

## Parameters

| Parameter           | Description                                                                                              | Default Value | Parameter in Workflow File | Type     |
|---------------------|----------------------------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Output file**     | Location of the output data file. If this attribute is set, then the “Location” slot is not taken into account. |               | **url-out**                | _string_ |
| **Output file suffix** | This suffix will be used for generating the output file name.                                            |               | **url-suffix**             | _string_ |
| **Existing file**   | If a target file already exists, you can specify how it should be handled: either overwritten, renamed, or appended (if supported by file format). | Rename        | **write-mode**             | _numeric_ |
|                     | Available values are:                                                                                      |               |                            |          |
|                     | * 0 - for overwrite                                                                                        |               |                            |          |
|                     | * 1 - for append                                                                                           |               |                            |          |
|                     | * 2 - for rename                                                                                           |               |                            |          |
| **Accumulate objects** | Accumulates all incoming data in one file or creates separate files for each input. In the latter case, an incremental numerical suffix is added to the file name. | True          | **accumulate**             | _boolean_ |

## Input/Output Ports

The element has 1 _input port_:

| Slot In GUI    | Slot in Workflow File | Type      |
|----------------|-----------------------|-----------|
| **Name in GUI:** _Sequence_ | **Name in Workflow File:** in-sequence |           |
| **Sequence**   | **sequence**          | _sequence_ |
| **Location**   | **url**               | _string_   |
| **FASTA header** | **fasta-header**    | _string_   |