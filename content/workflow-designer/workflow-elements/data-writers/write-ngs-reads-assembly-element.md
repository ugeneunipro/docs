---
title: "Write NGS Reads Assembly Element"
weight: 400
---

# Write NGS Reads Assembly Element

This element processes message(s) containing assembled reads data and saves the data to the specified file(s) in one of the suitable formats (SAM, BAM, or UGENEDB).

**Element type:** write-assembly

### Parameters

| Parameter              | Description                                                                                              | Default value | Parameter in Workflow File | Type    |
|------------------------|----------------------------------------------------------------------------------------------------------|---------------|----------------------------|---------|
| **Data storage**       | Specifies where to store workflow results: local file system or a database.                               |               | data-storage               | _string_ |
| **Document format**    | The document format of the output file.                                                                   | bam           | document-format            | _string_ |
| **Build index (BAM only)** | Builds a BAM index for the target BAM file. The file .bai will be created in the same directory.     | True          | build-index                | _boolean_ |
| **Output file**        | Location of the output data file. If this attribute is set, the "Location" slot in the port will not be used. |               | out-url                    | _string_ |
| **Output file suffix** | This suffix will be used for generating the output file name.                                            |               | url-suffix                 | _string_ |
| **Existing file**      | Specifies how an existing target file should be handled: overwritten, renamed, or appended (if supported by file format). If the Rename option is chosen, the existing file will be renamed. | Rename        | write-mode                 | _numeric_ |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Assembly_

**Name in Workflow File:** in-assembly

**Slots:**

| Slot in GUI   | Slot in Workflow File | Type       |
|---------------|-----------------------|------------|
| **Assembly data** | assembly              | _assembly_ |
| **Location**  | url                   | _string_   |