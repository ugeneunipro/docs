---
title: "Remove Duplicates in BAM Files Element"
weight: 1200
---

# Remove Duplicates in BAM Files Element

Remove PCR duplicates from BAM files using SAMTools rmdup.

**Element type:** rmdup-bam

Parameters
----------

| Parameter                       | Description                                                                                          | Default Value          | Parameter in Workflow File | Type       |
|---------------------------------|------------------------------------------------------------------------------------------------------|------------------------|----------------------------|------------|
| **Output directory**            | Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file. | Input file             |                            |            |
| **out-mode**                    |                                                                                                      |                        |                            | _numeric_  |
| **Output BAM name**             | A name for the output file. If the default or empty value is provided, the output name is the name of the first file with an additional extension. |                        | **out-name**               | _string_   |
| **Remove for single-end reads** | Remove duplicates for single-end reads. By default, the command works for paired-end reads only (-s). | False                  | **remove-single-end**      | _boolean_  |
| **Treat as single-end**         | Treat paired-end reads as single-end reads (-S).                                                     | False                  | **treat_reads**            | _boolean_  |

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input File  
**Name in Workflow File:** in-file

| Slot In GUI  | Slot in Workflow File | Type     |
|--------------|------------------------|----------|
| **Source URL** | **url**               | _string_ |

And 1 _output port_:

**Name in GUI:** Output File  
**Name in Workflow File:** out-file

| Slot In GUI  | Slot in Workflow File | Type     |
|--------------|------------------------|----------|
| **Source URL** | **url**               | _string_ |