---
title: "Write Sequence Element"
weight: 600
---

# Write Sequence Element

This element receives message(s) with sequence data and, optionally, associated annotation data. It saves the data to the specified file(s) in one of the appropriate formats (GenBank, FASTA, etc.).

**Element type:** write-sequence

## Parameters

| Parameter               | Description                                                                                                           | Default value | Parameter in Workflow File | Type                     |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|--------------------------|
| **Data storage**        | Place to store workflow results: local file system or a database.                                                     |               | data-storage               | _string_                 |
| **Output file**         | Location of the output data file. If this attribute is set, the “Location” slot is not taken into account.            |               | url-out                    | _string_                 |
| **Output file suffix**  | This suffix will be used for generating the output file name.                                                         |               | url-suffix                 | _string_                 |
| **Existing file**       | Specifies how to handle existing target files: overwrite, rename, or append (if supported by the file format).        | Rename        | write-mode                 | _numeric_                |
| **Document format**     | Format of the output file.                                                                                            | fasta         | document-format            | _string_                 |
| **Accumulate objects**  | Accumulates all incoming data in one file or creates separate files for each input. Adds an incremental numerical suffix to the filename if separate files are created. | True          | accumulate                 | _boolean_                |
| **Split sequence**      | Splits each incoming sequence into several parts.                                                                    | 1             | split                      | _numeric_                |

Available values for **Existing file** (write-mode):

- 0 - Overwrite
- 1 - Append
- 2 - Rename

Available formats for **Document format**:

- fasta
- fastq
- genbank
- raw

## Input/Output Ports

The element has 1 input port:

| Name in GUI     | Name in Workflow File | Type                     | Slots in GUI      | Slots in Workflow File   |
|-----------------|-----------------------|--------------------------|-------------------|--------------------------|
| **Sequence**    | in-sequence           | _sequence_               | **Sequence**      | sequence                 |
|                 |                       |                          | **Location**      | url                      |
|                 |                       |                          | **Set of annotations** | annotations            |
