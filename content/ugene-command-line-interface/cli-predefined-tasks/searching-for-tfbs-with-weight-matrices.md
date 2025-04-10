---
title: "Searching for TFBS with Weight Matrices"
weight: 2200
---

# Searching for TFBS with Weight Matrices

**Task Name:** pwm-search

This task searches for transcription factor binding sites (TFBS) using position weight matrices (PWM) and saves the identified regions as annotations.

**Parameters:**

- _seq_ — a semicolon-separated list of input sequence files in which to search for TFBS. \[String, Required\]

- _matrix_ — a semicolon-separated list of the input PWMs. \[String, Required\]

- _out_ — the output Genbank file.

- _name_ — the name of the annotated regions. \[String, Optional, Default: “misc\_feature”\]

- _min-score_ — the minimum percentage score to detect TFBS. \[Number, Optional, Default: 85\]

- _strand_ — strands to search in. \[Number, Optional, Default: 0\]

  The following values are available:

  * 0 (both strands)
  * 1 (direct strand)
  * -1 (complement strand)

**Example:**

ugene pwm-search --seq=input.fa --matrix=Aro80.pwm;Aft1.pwm --out=res.gb