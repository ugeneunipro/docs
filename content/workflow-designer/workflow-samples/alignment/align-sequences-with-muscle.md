---
title: "Align Sequences with MUSCLE"
weight: 100
---

# Align Sequences with MUSCLE

This workflow performs multiple sequence alignment using the MUSCLE algorithm and saves the resulting alignment in a Stockholm document. Source data can be in any format containing sequences or alignments.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, please consult the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Align Sequences with MUSCLE" can be found in the "Alignment" section of the Workflow Designer samples.

##### Workflow Image

The workflow appears as follows:

![](/images/65930229/65930230.png)

##### Workflow Wizard

The wizard contains 2 pages.

1. **Input MSA(s)**: On this page, you must input multiple alignment file(s).

   ![](/images/65930229/65930231.png)

2. **Align Sequences with MUSCLE**: On this page, you can modify MUSCLE and output parameters.

   ![](/images/65930229/65930232.png)

   The following parameters are available:

   | Parameter            | Description                                                                                                                                                           |
   |----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   | **Mode**             | Selector of preset configurations, offering you the choice to optimize accuracy, speed, or a compromise between the two. The default favors accuracy.                  |
   | **Stable order**     | Do not rearrange aligned sequences (-stable switch of MUSCLE). Otherwise, MUSCLE rearranges sequences so that similar sequences are adjacent in the output file. This makes the alignment easier to evaluate by eye. |
   | **Max iterations**   | Maximum number of iterations.                                                                                                                                          |
   | **Region to align**  | Whole alignment or column range, e.g., 1..100.                                                                                                                         |
   | **Result alignment** | Location of the output data file. If this attribute is set, the slot "Location" in the port will not be used.                                                          |
   | **Document format**  | Document format of the output file.                                                                                                                                    |