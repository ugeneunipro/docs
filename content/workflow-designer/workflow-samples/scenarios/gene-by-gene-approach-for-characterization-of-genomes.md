---
title: "Gene-by-gene Approach for Characterization of Genomes"
weight: 400
---

# Gene-by-gene Approach for Characterization of Genomes

Suppose you have genomes and you want to characterize them. One of the ways to do that is to build a table of what genes
are in each genome and what are not there.

## Step-by-step Instructions

1. Create a local BLAST database of your genome sequence/contigs. One DB per genome.
2. Create a file with sequences of genes you want to explore. This file will be the input file for the workflow.
3. Set up location and name of the BLAST DB you created for the first genome.
4. Set up output files: report location and (optionally) a file with annotated (via BLAST) sequences. You can delete the
   **Write Sequence** element if you don’t need output sequences.
5. Run the workflow.
6. Run the workflow again on the same input and output files, changing only the BLAST DB for each genome you have.

As a result, you'll get a report file with “Yes” and “No” values:

- “Yes” means the gene is found in the genome.
- “No” might mean the gene is missing, but it's recommended to analyze all the “No” cases using the annotated files.
  Just open the file and find the sequence by gene name.

---

## How to Use This Sample

If you haven't used workflow samples in UGENE before, refer
to [How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows).

---

## Workflow Sample Location

The workflow sample **Gene-by-gene Approach for Characterization of Genomes** is in the **Scenarios** section of the
Workflow Designer samples.

---

## Workflow Image

The workflow looks as follows:

![Workflow image](/images/65930545/65930546.png)

---

## Workflow Wizard

The wizard includes 3 pages:

### 1. Input Sequence(s)

On this page you must input sequence(s):

![Input](/images/65930545/65930547.png)

---

### 2. BLAST Search Settings

On this page, you can configure BLAST search parameters:

![BLAST settings](/images/65930545/65930548.png)

| **Parameter**           | **Description**                                        |
|-------------------------|--------------------------------------------------------|
| **Search type**         | Select type of BLAST search.                           |
| **Database Path**       | Path to folder with BLAST database files.              |
| **Database Name**       | Base name for BLAST DB files.                          |
| **Expected value**      | Statistical threshold for reporting matches (E-value). |
| **Annotate as**         | Name to use for result annotations.                    |
| **Gapped alignment**    | Whether to perform gapped alignment.                   |
| **Tool Path**           | Path to external BLAST tool.                           |
| **BLAST output**        | Path to the BLAST result file.                         |
| **BLAST output type**   | Format of the BLAST result file.                       |
| **Temporary directory** | Location to store temp files.                          |
| **Gap costs**           | Cost for creating/extending a gap.                     |
| **Match scores**        | Match reward and mismatch penalty.                     |

---

### 3. Output Data

On this page you can set output options:

![Output data](/images/65930545/65930549.png)
