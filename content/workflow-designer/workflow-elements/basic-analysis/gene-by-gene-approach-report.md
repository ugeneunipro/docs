---
title: "Gene-by-gene Approach Report"
weight: 1200
---

# Gene-by-gene Approach Report

Outputs a table of genes found in a reference sequence.

**Element type:** `genebygene-report-id`

---

## Parameters

| **Parameter**       | **Description**                                                                                           | **Default value** | **Parameter in Workflow File** | **Type**  |
|---------------------|-----------------------------------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| **Output file**     | Path to store the final report.                                                                           |                   | `output-file`                  | _string_  |
| **Annotation name** | Name of the annotation used to compare genes with reference genomes.                                      | `blast-result`    | `annotation_name`              | _string_  |
| **Existing file**   | How to handle an existing output file: `Merge`, `Overwrite`, or `Rename`.                                 | `Merge`           | `existing`                     | _string_  |
| **Identity cutoff** | Required identity between gene sequence length and annotation length (percent). BLAST identity is checked afterward. | `90.0000%`        | `identity`                     | _numeric_ |

---

## Input/Output Ports

### Input Port

| **Name in GUI**          | **Name in Workflow File** | **Slot in GUI**   | **Slot in Workflow File** | **Type**         |
|--------------------------|---------------------------|-------------------|---------------------------|------------------|
| Gene by gene report data | `in-data`                 | Input annotations | `gene-ann`                | _ann-table-list_ |
|                          |                           | Input sequences   | `gene-seq`                | _seq_            |