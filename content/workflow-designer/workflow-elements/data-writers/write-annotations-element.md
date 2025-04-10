---
title: "Write Annotations Element"
weight: 200
---

# Write Annotations Element

This element retrieves the message(s) containing annotation data and saves the data to the specified file(s) in one of the appropriate formats (GenBank, GTF, etc.). 

**Element type:** write-annotations

## Parameters

| Parameter                   | Description                                                                                  | Default value | Parameter in Workflow File | Type               |
|-----------------------------|----------------------------------------------------------------------------------------------|---------------|----------------------------|--------------------|
| **Data storage**            | Place to store workflow results: local file system or a database.                           |               | **data-storage**           | _string_           |
| **Output file**             | Location of the output data file. If this attribute is set, the "Location" slot in port will not be used. |               | **url-out**                | _string_           |
| **Output file suffix**      | This suffix will be used for generating the output file name.                                |               | **url-suffix**             | _string_           |
| **Existing file**           | If a target file already exists, specify how it should be handled: overwrite, rename, or append (if supported by file format). | Rename        | **write-mode**             | _numeric_          |
|                             | Available values are:                                                                        |               |                            |                    |
|                             | * 0 - Overwrite                                                                             |               |                            |                    |
|                             | * 1 - Append                                                                                |               |                            |                    |
|                             | * 2 - Rename                                                                                |               |                            |                    |
| **Document format**         | Document format of the output file.                                                          | genbank       | **document-format**        | _string_           |
|                             | Available values are:                                                                        |               |                            |                    |
|                             | * CSV                                                                                       |               |                            |                    |
|                             | * GenBank                                                                                   |               |                            |                    |
|                             | * GFF                                                                                       |               |                            |                    |
| **Merge annotations table** | If true, all annotation tables from the dataset will be merged into one. The Annotation table name parameter value will be used as the result annotation table's name. | False         | **merge**                  | _boolean_          |

## Input/Output Ports

The element has 1 [input port](http://ugene.unipro.ru/documentation/wd_manual/introduction/schema_terms.html#term-input-port):

**Name in GUI:** _Input annotations_

**Name in Workflow File:** in-annotations

| Slot in GUI          | Slot in Workflow File | Type                   |
|----------------------|-----------------------|------------------------|
| **Set of annotations** | **annotations**        | _annotation-table-list_ |
| **Sequence**           | **sequence**          | _sequence_              |
| **Source URL**         | **url**               | _string_                |