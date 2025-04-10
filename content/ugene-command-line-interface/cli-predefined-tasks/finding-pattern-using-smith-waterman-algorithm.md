---
title: "Finding Patterns Using the Smith-Waterman Algorithm"
weight: 600
---

# Finding Patterns Using the Smith-Waterman Algorithm

**Task Name:** find-sw

Searches for a pattern in a nucleotide or protein sequence using the Smith-Waterman algorithm and saves the regions found as annotations.

**Parameters:**

_in_ — Input sequence file. \[String, Required\]

_out_ — Output file with the annotations. \[String, Required\]

_name_ — Name of the annotated regions. \[String, Optional, Default: “misc\_feature”\]

_ptrn_ — Subsequence pattern to search for (e.g., _AGGCCT_). \[String, Required\]

_score_ — Percent identity between the pattern and a subsequence. \[Number, Optional, Default: 90\]

_matrix_ — Scoring matrix. \[String, Optional, Default: “Auto”\]

Among others, the following values are available:

- blosum62
- dna
- rna
- dayhoff
- gonnet
- pam250
- etc.

The available matrices are stored in the $UGENE\\data\\weight\_matrix directory.

_filter_ — Results filtering strategy. \[String, Optional, Default: “filter-intersections”\]

The following values are available:

- filter-intersections
- none

**Example:**

ugene find-sw --in=human\_T1.fa --out=sw.gb --ptrn=TGCT --filter=none