---
title: "Aligning with T-Coffee"
weight: 1
---


# Aligning with T-Coffee

**Task Name:** align-tcoffee

Create alignment with T-Coffee. T-Coffee is a collection of tools for computing, evaluating and manipulating multiple alignments of DNA, RNA, Protein Sequences.

T-Coffee is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

_gap-ext-penalty_ - Gap Extension Penalty. Positive values give rewards to gaps and prevent the alignment of unrelated segments (using '0' by default) \[Number\]

_gap-open-penalty_ - Gap Open Penalty. Must be negative, best matches get a score of 1000 (using '-50' by default) \[Number\]

_iter-max_ - Number of iteration on the progressive alignment: 0 - no iteration (default), -1 - Nseq iterations (using '0' by default) \[Number\]

_toolpath_ - T-Coffee location (using the path specified in UGENE by default) \[String\]

_tmpdir_ - Directory to store temporary files (using UGENE temporary directory by default) \[String\]

_in_ - Input alignment \[Url datasets\]

_format_ - Document format of output alignment (using 'clustal' by default) \[String\]

_out_ - Output alignment \[String\]

**Example:**

ugene align-tcoffee  --in=test.aln --out=test\_out.aln --format=clustal
