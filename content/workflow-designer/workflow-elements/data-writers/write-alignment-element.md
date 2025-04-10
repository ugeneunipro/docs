---
title: "Write Alignment Element"
weight: 100
---

# Write Alignment Element

This element receives message(s) with alignment data and saves the data to the specified file(s) in one of the multiple sequence alignment formats supported by UGENE (ClustalW, FASTA, etc.).

**Element type:** write-msa

## Parameters

| Parameter          | Description                                                                                                                                       | Default value | Parameter in Workflow File | Type    |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|---------------|-----------------------------|---------|
| **Data storage**   | The place to store workflow results: local file system or a database.                                                                              |               | **data-storage**           | _string_|
| **Document format**| The format of the output file.                                                                                                                     | clustal       | **document-format**        | _string_|
|                    | Available values are:                                                                                                                              |               |                             |         |
|                    | * clustal                                                                                                                                          |               |                             |         |
|                    | * mega                                                                                                                                             |               |                             |         |
|                    | * msf                                                                                                                                              |               |                             |         |
|                    | * sam                                                                                                                                              |               |                             |         |
|                    | * srfasta                                                                                                                                          |               |                             |         |
|                    | * stockholm                                                                                                                                         |               |                             |         |
| **Output file**    | Location of the output data file. If this parameter is set, then the “Location” slot is not considered.                                           |               | **url-out**                | _string_|
| **Output file suffix** | This suffix will be used for generating the output file name.                                                                                  |               | **url-suffix**             | _string_|
| **Existing file**  | If a target file already exists, you can specify how it should be handled: either overwritten, renamed, or appended (if supported by the file format). | Rename        | **write-mode**             | _numeric_|
|                    | Available values are:                                                                                                                              |               |                             |         |
|                    | * 0 - for overwrite                                                                                                                                |               |                             |         |
|                    | * 1 - for append                                                                                                                                   |               |                             |         |
|                    | * 2 - for rename                                                                                                                                   |               |                             |         |

## Input/Output Ports

The element has 1 _input port_:

| Slot In GUI             | Slot in Workflow File | Type  |
|-------------------------|-----------------------|-------|
| **Name in GUI:**        |                       |       |
| _Multiple sequence alignment_ | in-msa               |       |
| **Slots:**              |                       |       |
| **MSA**                 | **msa**               | _msa_ |
| **Location**            | **url**               | _string_ |