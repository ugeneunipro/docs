---
title: "Building PFM"
weight: 1900
---


# Building PFM

**Task Name:** pfm-build

Builds a position frequency matrix from a multiple sequence alignment file.

**Parameters:**

_in_ — semicolon-separated list of input MSA files. \[String, Required\]

_out_ — output file. \[String, Required\]

_type_ — type of the matrix. \[Boolean, Optional, Default: false\]

The following values are available:

*   *   true (dinucleic type)
    *   false (mononucleic type)

Dinucleic matrices are more detailed, while mononucleic ones are more useful for small input data sets.

**Example:**

ugene pfm-build --in=COI.aln --out=result.pfm
