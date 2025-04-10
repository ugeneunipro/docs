---
title: "Aligning with MUSCLE"
weight: 1300
---

# Aligning with MUSCLE

**Task Name:** align

Performs multiple sequence alignment with the MUSCLE algorithm and saves the resulting alignment to a file. Source data can be of any format containing sequences or alignments.

**Parameters:**

| Parameter      | Description                                                                                                                                                                               | Default Value       | Type    |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------|---------|
| _in_           | Input alignment \[Url datasets\]                                                                                                                                                          |                     |         |
| _max-iterations_ | Maximum number of iterations (using '2' by default)                                                                                                                                     | 2                   | Number  |
| _mode_         | Selector of preset configurations, that give you the choice of optimizing accuracy, speed, or some compromise between the two. The default favors accuracy (using 'MUSCLE default' by default) | MUSCLE default      | String  |
| _range_        | Whole alignment or column range, e.g., 1..100 (using 'Whole alignment' by default)                                                                                                        | Whole alignment     | String  |
| _stable_       | Do not rearrange aligned sequences (using 'True' by default)                                                                                                                              | True                | Boolean |
| _format_       | Document format of output alignment (using 'clustal' by default)                                                                                                                          | clustal             | String  |
| _out_          | Output alignment \[String\]                                                                                                                                                               |                     |         |

**Example:**

```bash
ugene align --in=test.aln --out=test_out.aln --format=clustal