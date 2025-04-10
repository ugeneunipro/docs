---
title: "Searching for TFBS with PFM"
weight: 2000
---

# Searching for TFBS with PFM

**Task Name:** pfm-search

This task searches for transcription factor binding sites (TFBS) using position weight matrices (PWM) converted from input position frequency matrices (PFM) and saves the identified regions as annotations.

**Parameters:**

- _seq_ — A semicolon-separated list of input sequence files to search for TFBS. \[String, Required\]

- _matrix_ — A semicolon-separated list of the input PFM files. \[String, Required\]

- _out_ — The output Genbank file.

- _name_ — The name of the annotated regions. \[String, Optional, Default: "misc_feature"\]

- _type_ — The type of the matrix. \[Boolean, Optional, Default: false\]

  The following values are available:
  
  - true (dinucleic type)
  - false (mononucleic type)

  Dinucleic matrices provide more detail, while mononucleic matrices are more useful for smaller input datasets.

- _algo_ — The algorithm used to convert a PFM to a PWM. \[String, Optional, Default: "Berg and von Hippel"\]

  The following values are available:
  
  - Berg and von Hippel
  - Log-odds
  - Match
  - NLG

- _score_ — The minimum percentage score to detect TFBS. \[Number, Optional, Default: 85\]

- _strand_ — The strands to search in. \[Number, Optional, Default: 0\]

  The following values are available:
  
  - 0 (both strands)
  - 1 (direct strand)
  - -1 (complement strand)

**Example:**

```bash
ugene pfm-search --seq=in.fa --matrix=MA0265.1.pfm;MA0266.1.pfm --out=res.gb