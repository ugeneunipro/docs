---
title: "Aligning with T-Coffee"
weight: 1800
---

# Aligning with T-Coffee

**Task Name:** align-tcoffee

Create alignments with T-Coffee. T-Coffee is a collection of tools for computing, evaluating, and manipulating multiple alignments of DNA, RNA, and Protein sequences.

T-Coffee is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

- _gap-ext-penalty_: Gap Extension Penalty. Positive values give rewards to gaps and prevent the alignment of unrelated segments (default is '0') \[Number\]

- _gap-open-penalty_: Gap Open Penalty. Must be negative; best matches get a score of 1000 (default is '-50') \[Number\]

- _iter-max_: Number of iterations on the progressive alignment: 0 - no iteration (default), -1 - Nseq iterations (default is '0') \[Number\]

- _toolpath_: T-Coffee location (default is the path specified in UGENE) \[String\]

- _tmpdir_: Directory to store temporary files (default is UGENE temporary directory) \[String\]

- _in_: Input alignment \[URL datasets\]

- _format_: Document format of output alignment (default is 'clustal') \[String\]

- _out_: Output alignment \[String\]

**Example:**

```
ugene align-tcoffee --in=test.aln --out=test_out.aln --format=clustal