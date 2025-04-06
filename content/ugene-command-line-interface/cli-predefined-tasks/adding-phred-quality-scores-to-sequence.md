---
title: "Adding Phred Quality Scores to Sequence"
weight: 1
---


# Adding Phred Quality Scores to Sequence

**Task Name:** join-quality

Adds Phread quality scores to a sequence and saves the result to the output FASTQ file.

**Parameters:**

_in_ — input sequence file. \[String, Required\]

_quality_ — input Phred quality scores file. \[String, Required\]

_out_ — output FASTQ file. \[String, Required\]

**Example:**

ugene join-quality --in=e\_coli.fa --quality=e\_coli.qual --out=res.fastq
