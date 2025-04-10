---
title: "Adding Phred Quality Scores to Sequence"
weight: 700
---

# Adding Phred Quality Scores to Sequence

**Task Name:** join-quality

Adds Phred quality scores to a sequence and saves the result to the output FASTQ file.

**Parameters:**

| Parameter | Description | Type | Requirement |
|-----------|-------------|------|-------------|
| _in_ | Input sequence file. | String | Required |
| _quality_ | Input Phred quality scores file. | String | Required |
| _out_ | Output FASTQ file. | String | Required |

**Example:**

ugene join-quality --in=e\_coli.fa --quality=e\_coli.qual --out=res.fastq