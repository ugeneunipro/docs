---
title: "Aligning with MUSCLE"
weight: 1
---


# Aligning with MUSCLE

**Task Name:** align

Performs multiple sequence alignment with MUSCLE algorithm and saves the resulting alignment to file. Source data can be of any format containing sequences or alignments.

**Parameters:**

_in -_ Input alignment \[Url datasets\]_max-iterations -_ Maximum number of iterations (using '2' by default) \[Number\]_mode -_ Selector of preset configurations, that give you the choice of optimizing accuracy, speed,or some compromise between the two. The default favors accuracy (using 'MUSCLE default' by default) \[Number\]_range -_ Whole alignment or column range e.g. 1..100 (using 'Whole alignment' by default) \[String\]_stable -_ Do not rearrange aligned sequences (using 'True' by default) \[Boolean\]_format -_ Document format of output alignment (using 'clustal' by default) \[String\]_out -_ Output alignment \[String\]

**Example:**

ugene align  --in=test.aln --out=test\_out.aln --format=clustal
