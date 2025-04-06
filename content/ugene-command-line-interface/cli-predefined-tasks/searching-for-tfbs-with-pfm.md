---
title: "Searching for TFBS with PFM"
weight: 1
---


# Searching for TFBS with PFM

**Task Name:** pfm-search

Searches for transcription factor binding sites (TFBS) with position weight matrices (PWM) converted from input position frequency matrices (PFM) and saves the regions found as annotations.

**Parameters:**

_seq_ — semicolon-separated list of input sequence files to search TFBS in. \[String, Required\]

_matrix_ — semicolon-separated list of the input PFM. \[String, Required\]

_out_ — output Genbank file.

_name_ — name of the annotated regions. \[String, Optional, Default: “misc\_feature”\]

_type_ — type of the matrix. \[Boolean, Optional, Default: false\]

The following values are available:

*   *   true (dinucleic type)
    *   false (mononucleic type)

Dinucleic matrices are more detailed, while mononucleic ones are more useful for small input data sets.

_algo_ — algorithm used to convert a PFM to a PWM. \[String, Optional, Default: “Berg and von Hippel”\]

The following values are available:

*   *   Berg and von Hippel
    *   Log-odds
    *   Match
    *   NLG

_score_ — minimum percentage score to detect TFBS. \[Number, Optional, Default: 85\]

_strand_ — strands to search in. \[Number, Optional, Default: 0\]

The following values are available:

*   *   0 (both strands)
    *   1 (direct strand)
    *   \-1 (complement strand)

**Example:**

ugene pfm-search --seq=in.fa --matrix=MA0265.1.pfm;MA0266.1.pfm --out=res.gb
