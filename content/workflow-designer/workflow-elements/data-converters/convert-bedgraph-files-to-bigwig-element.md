---
title: "Convert bedGraph Files to bigWig Element"
weight: 100
---

# Convert bedGraph Files to bigWig Element

Convert bedGraph files to bigWig.

**Element type:** bgtbw-bam

## Parameters

| Parameter            | Description                                                                                                                                          | Default value | Parameter in Workflow File | Type      |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Output directory** | Select an output directory. Options:<br>Custom – use 'Custom directory' parameter<br>Workflow – internal directory<br>Input file – directory of the input file | Input file    | **out-mode**               | _numeric_ |
| **Custom directory** | Specify the output directory path.                                                                                                                   |               | **custom-dir**             | _string_  |
| **Genome**           | File with genome length.                                                                                                                             | human.hg18    | **genome**                 | _string_  |
| **Output name**      | Output filename. If left empty, the first input file name is used with an additional extension.                                                      |               | **out-name**               | _string_  |
| **Block size**       | Number of items to bundle in R-tree.                                                                                                                 | 256           | **bs**                     | _numeric_ |
| **Items per slot**   | Data points bundled at the lowest level.                                                                                                             | 1024          | **its**                    | _numeric_ |
| **Uncompressed**     | If true, do not use compression.                                                                                                                     | False         | **unc**                    | _boolean_ |

## Input/Output Ports

| Port Name (GUI)    | Workflow File Name | Slots                             |
|--------------------|--------------------|-----------------------------------|
| **BedGraph files** | `in-file`          | **Source URL** → `url` (_string_) |
| **BigWig files**   | `out-file`         | **Source URL** → `url` (_string_) |
