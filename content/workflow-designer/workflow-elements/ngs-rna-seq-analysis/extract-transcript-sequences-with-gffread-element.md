---
title: "Extract Transcript Sequences with gffread Element"
weight: 300
---

# Extract Transcript Sequences with gffread Element

This workflow element uses **gffread** to extract transcript sequences from provided genomic sequences and GFF/GTF
annotation files.

**Element type:** `gffread`

---

## Parameters

| **Parameter**        | **Description**                                             | **Default Value** | **Parameter in Workflow File** | **Type** |
|----------------------|-------------------------------------------------------------|-------------------|--------------------------------|----------|
| **Output sequences** | Path to the output FASTA file with the extracted sequences. | *(not set)*       | `url-out`                      | _string_ |

---

## Input/Output Ports

### Input Port

| **Name in GUI**     | **Name in Workflow File** | **Slot**             | **Slot in Workflow File** | **Type** |
|---------------------|---------------------------|----------------------|---------------------------|----------|
| `Input transcripts` | `in-data`                 | Genomic sequence url | `genome`                  | _string_ |
|                     |                           | Transcripts url      | `transcripts`             | _string_ |

### Output Port

| **Name in GUI**           | **Name in Workflow File** | **Slot**  | **Slot in Workflow File** | **Type** |
|---------------------------|---------------------------|-----------|---------------------------|----------|
| `Extracted sequences url` | `extracted-data`          | sequences | `sequences`               | _string_ |

---

## Example

You can use this element in a workflow to extract coding sequences (CDS) or full transcript sequences using a reference
genome and GFF/GTF file.

```bash
ugene workflow run \
  --element gffread \
  --genome genome.fa \
  --transcripts annotations.gtf \
  --url-out transcripts.fa
  ```

This will output transcripts.fa containing the sequences of all transcripts described in annotations.gtf, extracted from
genome.fa.
