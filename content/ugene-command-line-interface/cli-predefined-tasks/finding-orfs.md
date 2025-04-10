---
title: "Finding ORFs"
weight: 400
---

# Finding ORFs

**Task Name:** find-orfs

This task involves searching for Open Reading Frames (ORFs) in nucleotide sequences and saving the identified regions as annotations.

**Parameters:**

- **_in_** — A semicolon-separated list of input files. \[String, Required\]

- **_out_** — An output file containing the annotations. \[String, Required\]

- **_name_** — The name of the annotated regions. \[String, Optional, Default: "ORF"\]

- **_min-length_** — Ignores ORFs shorter than the specified length. \[String, Optional, Default: 100\]

- **_require-stop-codon_** — Ignores boundary ORFs that extend beyond the search region (i.e., have no stop codon within the range). \[Boolean, Optional, Default: false\]

- **_require-init-codon_** — Allows ORFs to start with any codon other than a terminator. \[Boolean, Optional, Default: true\]

- **_allow-alternative-codons_** — Allows ORFs to start with alternative initiation codons according to the current translation table. \[Boolean, Optional, Default: false\]

**Example:**

```bash
ugene find-orfs --in=human_T1.fa --out=result.gb --require-init-codon=false