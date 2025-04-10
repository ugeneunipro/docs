---
title: "Sort BAM Files Element"
weight: 1400
---

# Sort BAM Files Element

Sort BAM Files using SAMTools Sort.

**Element type:** Sort-bam

## Parameters

| Parameter             | Description                                                                                                                                                                   | Default Value | Parameter in Workflow File | Type    |
|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|---------|
| **Output directory**  | Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file. | Input file    |                            |         |
| **out-mode**          | _numeric_                                                                                                                                                                     |               | out-mode                   | numeric |
| **Custom directory**  | Specify the output directory.                                                                                                                                                 |               | custom-dir                 | string  |
| **Output BAM name**   | A name for the output file. If the default or an empty value is provided, the output name is the name of the first file with an additional extension.                         |               | out-name                   | string  |
| **Build index**       | Build index for the sorted file with SAMTools index.                                                                                                                          | human.hg18    | index                      | boolean |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** BAM File

**Name in Workflow File:** in-file

**Slots:**

| Slot In GUI | Slot in Workflow File | Type   |
|-------------|------------------------|--------|
| **Source URL** | **url**               | string |

And 1 _output port_:

**Name in GUI:** Sorted BAM File

**Name in Workflow File:** out-file

**Slots:**

| Slot In GUI | Slot in Workflow File | Type   |
|-------------|------------------------|--------|
| **Source URL** | **url**               | string |