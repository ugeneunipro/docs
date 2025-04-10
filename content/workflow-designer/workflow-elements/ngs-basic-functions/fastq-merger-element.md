---
title: "FASTQ Merger Element"
weight: 500
---

# FASTQ Merger Element

Merges input sequences into one output file.

**Element type:** `MergeFastq`

---

## Parameters

| **Parameter**        | **Description**                                                                                                                                                                             | **Default Value** | **Parameter in Workflow File** | **Type** |
|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------------------------------|----------|
| **Output directory** | Select an output directory. Custom – specify the output directory in the 'Custom directory' parameter. Workflow – internal workflow directory. Input file – the directory of the input file. | *(not set)*       | `out-mode`                     | _string_ |
| **Output file name** | The name of the output file. If the default or an empty value is provided, the output name is the name of the first file with an additional extension.                                      | *(not set)*       | `out-name`                     | _string_ |

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

---

## Example

```bash
ugene workflow run \
  --element MergeFastq \
  --url input1.fastq,input2.fastq,input3.fastq \
  --out-name merged_output.fastq
```

This command merges multiple FASTQ files into one. Use `--out-mode` and `--custom-dir` if you want to set a specific output location.