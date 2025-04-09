---
title: "Searching for TFBS with Weight Matrices"
weight: 2200
---


# Searching for TFBS with Weight Matrices

**Task Name:** pwm-search

Searches for transcription factor binding sites (TFBS) with position weight matrices (PWM) and saves the regions found as annotations.

**Parameters:**

_seq_ — semicolon-separated list of input sequence files to search TFBS in. \[String, Required\]

_matrix_ — semicolon-separated list of the input PWM. \[String, Required\]

_out_ — output Genbank file.

_name_ — name of the annotated regions. \[String, Optional, Default: “misc\_feature”\]

_min-score_ — minimum percentage score to detect TFBS. \[Number, Optional, Default: 85\]

_strand_ — strands to search in. \[Number, Optional, Default: 0\]

The following values are available:

*   *   0 (both strands)
    *   1 (direct strand)
    *   \-1 (complement strand)

**Example:**

ugene pwm-search --seq=input.fa --matrix=Aro80.pwm;Aft1.pwm --out=res.gb
