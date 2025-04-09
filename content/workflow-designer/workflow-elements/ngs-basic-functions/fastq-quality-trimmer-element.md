---
title: "FASTQ Quality Trimmer Element"
weight: 600
---

# FASTQ Quality Trimmer Element

The workflow scans each input sequence from the end to find the first position where the quality is greater or equal to
the minimum quality threshold. Then it trims the sequence to that position. If the whole sequence has quality less than
the threshold or the length of the output sequence is less than the minimum length threshold, then the sequence is
skipped.

**Element type:** `QualityTrim`

---

## Parameters

| **Parameter**         | **Description**                                                                                                                                                                              | **Default Value** | **Parameter in Workflow File** | **Type**  |
|-----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| **Output directory**  | Select an output directory. Custom – specify the output directory in the 'Custom directory' parameter. Workflow – internal workflow directory. Input file – the directory of the input file. | Input file        | `out-mode`                     | _numeric_ |
| **Custom directory**  | Specify the output directory.                                                                                                                                                                | *(not set)*       | `custom-dir`                   | _string_  |
| **Output file name**  | A name of an output file. If empty, the name of the first file will be used with an additional extension.                                                                                    | *(not set)*       | `out-name`                     | _string_  |
| **Quality threshold** | Quality threshold for trimming.                                                                                                                                                              | 30                | `qual-id`                      | _numeric_ |
| **Min Length**        | Too short reads are discarded by the filter.                                                                                                                                                 | 0                 | `len-id`                       | _numeric_ |
| **Trim both ends**    | Trim both ends of a read. Usually, set to `True` for Sanger sequencing and `False` for NGS.                                                                                                  | True              | `both-ends`                    | _boolean_ |

---

## Input/Output Ports

### Input Port

| **Name in GUI** | **Name in Workflow File** | **Slot**   | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|------------|---------------------------|----------|
| Input File      | `in-file`                 | Source URL | `url`                     | _string_ |

### Output Port

| **Name in GUI** | **Name in Workflow File** | **Slot**   | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|------------|---------------------------|----------|
| Output File     | `out-file`                | Source URL | `url`                     | _string_ |
