---
title: "CASAVA FASTQ Filter Element"
weight: 100
---

# CASAVA FASTQ Filter Element

Reads in a FASTQ file produced by CASAVA 1.8 contain 'N' or 'Y' as part of an identifier.
'Y' indicates a read is filtered, 'N' indicates the read is not filtered. The workflow cleans up the filtered reads.

**Element type:** CASAVAFilter

## Parameters

| Parameter            | Description                                                                                                                                  | Default value | Parameter in Workflow File | Type      |
|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Output directory** | Select an output directory. `Custom` – use "Custom directory". `Workflow` – use internal directory. `Input file` – use input file directory. | Input file    | **out-mode**               | _numeric_ |
| **Custom directory** | Specify the output directory if "Custom" is selected.                                                                                        |               | **custom-dir**             | _string_  |
| **Output file name** | Name of the output file. If empty, the name of the first file with an added extension will be used.                                          |               | **out-name**               | _string_  |

## Input/Output Ports

| Port Name (GUI) | Workflow File Name | Slots                             |
|-----------------|--------------------|-----------------------------------|
| **Input File**  | `in-file`          | **Source URL** → `url` (_string_) |
| **Output File** | `out-file`         | **Source URL** → `url` (_string_) |
