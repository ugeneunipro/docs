---
title: "HMM2 Algorithm Element"
weight: 1400
---

# HMM2 Algorithm Element

Searches HMM signals in a sequence with one or more profile HMM2 and saves the results as annotations.

### Parameters in GUI

| Parameter                   | Description                                                                             | Default value       |
|-----------------------------|-----------------------------------------------------------------------------------------|---------------------|
| **Profile HMM**             | Semicolon-separated list of input HMM files. You must specify a value!                  |                     |
| **Min Length**              | Minimum length of a result region.                                                      | 10                  |
| **Max Length**              | Maximum length of a result region.                                                      | 1000                |
| **Filter by High E-value**  | Reports domains <= this E-value threshold in output (**hmmsearch** **–domE** option).   | 1e+1                |
| **Filter by Low Score**     | Reports domains >= this score cutoff in output (**hmmsearch** **–domT** option).        | 0.01                |
| **Number of Sequences**     | Specifies number of significant sequences. It is used for domain E-value calculations (**hmmsearch** **–domZ** option). | 1 (i.e. one input sequence) |


### Parameters in Schema File

**Type:** hmm2

| Parameter    | Parameter in the GUI  | Type    |
|--------------|-----------------------|---------|
| **min-len**  | **Min Length**        | _string_|
| **max-len**  | **Max Length**        | _string_|
| **hmm-profile** | **Profile HMM**    | _string_|
| **e-val**    | **Filter by High E-value** | _numeric_|
| **score**    | **Filter by Low Score** | _numeric_|
| **seqs-num** | **Number of Sequences** | _numeric_|