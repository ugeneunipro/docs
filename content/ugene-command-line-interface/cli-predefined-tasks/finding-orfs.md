---
title: "Finding ORFs"
weight: 1
---


# Finding ORFs

**Task Name:** find-orfs

Searches for Open Reading Frames (ORFs) in nucleotide sequences and saves the regions found as annotations.

**Parameters:**

_in_ — semicolon-separated list of input files. \[String, Required\]

_out_ — output file with the annotations. \[String, Required\]

_name_ — name of the annotated regions. \[String, Optional, Default: “ORF”\]

_min-length_ — ignores ORFs shorter than the specified length. \[String, Optional, Default: 100\]

_require-stop-codon_ — ignores boundary ORFs that last beyond the search region (i.e. have no stop codon within the range). \[Boolean, Optional, Default: false\]

_require-init-codon_ — allows ORFs starting with any codon other than terminator. \[Boolean, Optional, Default: true\]

_allow-alternative-codons_ — allows ORFs starting with alternative initiation codons, accordingly to the current translation table. \[Boolean, Optional, Default: false\]

**Example:**

ugene find-orfs --in=human\_T1.fa --out=result.gb --require-init-codon=false
