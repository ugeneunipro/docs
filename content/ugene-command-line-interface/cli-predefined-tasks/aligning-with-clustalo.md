---
title: "Aligning with ClustalO"
weight: 1
---


# Aligning with ClustalO

**Task Name:** align-clustalo

Create alignment with ClustalO. ClustalO is a general purpose multiple sequence alignment program for proteins.

ClustalO is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

_in -_ Input alignment \[Url datasets\]

_format -_ Document format of output alignment (using 'clustal' by default) \[String\]

_out -_ Output alignment \[String\]

_max-guidetree-iterations -_ Maximum number guidetree iterations (using '0' by default) \[Number\]

_max-hmm-iterations -_ Maximum number of HMM iterations (using '0' by default) \[Number\]

_iter -_ Number of (combined guide-tree/HMM) iterations (using '1' by default) \[Number\]

_toolpath -_ ClustalO location (using the path specified in UGENE by default) \[String\]

_auto -_ Set options automatically (might overwrite some of your options) (using 'False' by default) \[Boolean\]

_tmpdir -_ Directory to store temporary files (using UGENE temporary directory by default) \[String\]

**Example:**

ugene align-clustalw  --in=test.aln --out=test\_out.aln --format=clustal
