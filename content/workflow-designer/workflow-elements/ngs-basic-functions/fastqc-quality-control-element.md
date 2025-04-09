```markdown
---
title: "FastQC Quality Control Element"
weight: 700
---

# FastQC Quality Control Element

This element generates quality control reports for short read sequencing data using **FastQC**.

**Element type:** `fastqc`

---

## Parameters

| **Parameter**            | **Description**                                                                                          | **Default Value** | **Parameter in Workflow File** | **Type**   |
|--------------------------|----------------------------------------------------------------------------------------------------------|--------------------|--------------------------------|------------|
| **Output file**          | Name of the resulting FastQC report file. If not set, uses the input file name.                         | Input file         | `out-file`                     | _string_   |
| **List of adapters**     | Optional file with adapter sequences. Format: `name<TAB>sequence`. Lines starting with `#` are ignored. | *(not set)*        | `adapter`                      | _string_   |
| **List of contaminants** | Optional file with contaminants to screen for. Same format as adapters.                                 | *(not set)*        | `contaminants`                 | _string_   |

---

## Input/Output Ports

### Input Port

| **Name in GUI** | **Name in Workflow File** | **Slot**     | **Slot in Workflow File** | **Type**   |
|-----------------|----------------------------|--------------|----------------------------|------------|
| `Short reads`   | `in-file`                  | Source URL   | `url`                      | _string_   |

---

## Example

You can use this element to generate FastQC reports in a larger workflow:

```bash
ugene workflow run \
  --element fastqc \
  --url input_reads.fastq \
  --out-file fastqc_report.html
```

If you wish to customize adapter or contaminant lists:

```bash
ugene workflow run \
  --element fastqc \
  --url input.fastq \
  --adapter my_adapters.txt \
  --contaminants my_contaminants.txt \
  --out-file output_report.html
```

Adapter and contaminant files must contain tab-separated `name<tab>sequence` entries. Lines starting with `#` are
ignored.

```
