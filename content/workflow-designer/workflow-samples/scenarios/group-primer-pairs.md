---
title: "Group Primer Pairs"
weight: 500
---

# Group Primer Pairs

This workflow helps in determining different primer pairs that can be used in the same experiment.

First, you need to input a set of primer sequences in the following order: pair1\_direct\_primer, pair1\_reverse\_primer, pair2\_direct\_primer, pair2\_reverse\_primer, etc. This could be a multifasta file, for example.

Second, the primers are checked for heterodimer formations. If no such formations exist between all primers in two or more primer pairs, it means these pairs can be used simultaneously in the same reaction tube. Therefore, the workflow GROUPS these primer pairs.

However, please note that this workflow does not check the correctness of the primers themselves, for example, for hairpins, self-dimers, etc.

The result report of the analysis is stored by default in the "report.html" file.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

### Workflow Sample Location

The workflow sample "Group Primer Pairs" can be found in the "Scenarios" section of the Workflow Designer samples.

### Workflow Image

The workflow appears as follows:

![](/images/65930550/65930551.png)

### Workflow Wizard

The wizard consists of 2 pages.

1. **Input primers:** On this page, you must input primers.

    ![](/images/65930550/65930552.png)

2. **Output report file:** On this page, you can modify output parameters.

    ![](/images/65930550/65930553.png)