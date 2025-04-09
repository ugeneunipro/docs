---
title: "Cut Adapter Element"
weight: 200
---

# Cut Adapter Element

Removes adapter sequences.

**Element type:** CutAdaptFastq

## Parameters

| Parameter                              | Description                                                                                                                                                                                                                                                                                                          | Default value | Parameter in Workflow File | Type     |
|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Output directory**                   | Select an output directory. Custom – specify the output directory in the 'Custom directory' parameter. Workflow – internal workflow directory. Input file – the directory of the input file.                                                                                                                         | Input file    | **out-mode**               | _string_ |
| **Output file name**                   | A name of an output file. If default or empty value is provided, the output name is the name of the first file with an additional extension.                                                                                                                                                                         |               | **out-name**               | _string_ |
| **FASTA file with 3' adapters**        | A FASTA file with one or multiple sequences of adapter that were ligated to the 3' end. The adapter itself and anything that follows is trimmed. If the adapter sequence ends with the `$` character, the adapter is anchored to the end of the read and only found if it is a suffix of the read.                   |               | **adapters-url**           | _string_ |
| **FASTA file with 5' adapters**        | A FASTA file with one or multiple sequences of adapters that were ligated to the 5' end. If the adapter sequence starts with the character `^`, the adapter is anchored. Anchored adapters must appear in their entirety at the 5' end of the read (as a prefix). Otherwise, they may be partially or fully trimmed. |               | **front-url**              | _string_ |
| **FASTA file with 5' and 3' adapters** | A FASTA file with one or multiple sequences of adapters that were ligated to the 5' end or 3' end.                                                                                                                                                                                                                   |               | **anywhere-url**           | _string_ |

## Input/Output Ports

| Port Name (GUI) | Workflow File Name | Slots                             |
|-----------------|--------------------|-----------------------------------|
| **Input File**  | `in-file`          | **Source URL** → `url` (_string_) |
| **Output File** | `out-file`         | **Source URL** → `url` (_string_) |
