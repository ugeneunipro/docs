---
title: "Format Converting Sequences"
weight: 100
---


# Format Converting Sequences

**Task Name:** convert-seq

Converts a sequence from one format to another.

**Parameters:**

_in_ — input sequence file. \[String, Required\]

_out_ — name of the output file. \[String, Required\]

_format_ — format of the output file. \[String, Optional\]

The following values are available:

*   *   fasta
    *   fastq
    *   genbank
    *   gff
    *   raw

**Example:**

ugene convert-seq --in=human\_T1.fa --out=human\_T1.gbk --format=genbank
