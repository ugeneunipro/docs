---
title: "Finding Pattern Using Smith-Waterman Algorithm"
weight: 1
---


# Finding Pattern Using Smith-Waterman Algorithm

**Task Name:** find-sw

Searches for a pattern in a nucleotide or protein sequence using the Smith-Waterman algorithm and saves the regions found as annotations.

**Parameters:**

_in_ — input sequence file. \[String, Required\]

_out_ — output file with the annotations. \[String, Required\]

_name_ — name of the annotated regions. \[String, Optional, Default: “misc\_feature”\]

_ptrn_ — subsequence pattern to search for (e.g. _AGGCCT_). \[String, Required\]

_score_ — percent identity between the pattern and a subsequence. \[Number, Optional, Default: 90\]

_matrix_ — scoring matrix. \[String, Optional, Default: “Auto”\]

Among others the following values are available:

*   *   blosum62
    *   dna
    *   rna
    *   dayhoff
    *   gonnet
    *   pam250
    *   etc.

The matrices available are stored in the $UGENE\\data\\weight\_matrix directory.

_filter_ — results filtering strategy. \[String, Optional, Default: “filter-intersections”\]

The following values are available:

*   *   filter-intersections
    *   none

**Example:**

ugene find-sw --in=human\_T1.fa --out=sw.gb --ptrn=TGCT --filter=none
