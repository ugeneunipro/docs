---
title: "FASTQ Trimmer"
weight: 200
---

# FASTQ Trimmer

The workflow scans each input sequence from the end to find the first position where the quality is greater than or equal to the minimum quality threshold. Then it trims the sequence to that position. If the whole sequence has a quality less than the threshold, or if the length of the output sequence is less than the minimum length threshold, then the sequence is skipped.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, please refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "FASTQ Trimmer" can be found in the "Custom Elements" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:

![](/images/65930266/65930267.png)