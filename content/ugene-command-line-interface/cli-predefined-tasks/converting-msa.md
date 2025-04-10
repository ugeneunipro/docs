---
title: "Converting MSA"
weight: 200
---

# Converting MSA

**Task Name:** convert-msa

Converts a multiple sequence alignment file from one format to another.

**Parameters:**

_in_ — input multiple sequence alignment file. \[String, Required\]

_out_ — name of the output file. \[String, Required\]

_format_ — format of the output file. \[String, Optional\]

The following values are available:

*   clustal (default)
*   fasta
*   mega
*   msf
*   nexus
*   phylip-interleaved
*   phylip-sequential
*   stockholm

**Example:**

ugene convert-msa --in=CBS.sto --out=CBS --format=msf