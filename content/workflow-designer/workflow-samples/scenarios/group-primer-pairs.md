---
title: "Group Primer Pairs"
weight: 500
---


# Group Primer Pairs

The workflow helps determining different primer pairs that can be used in the same experiment.

First, you input a set of primers' sequences in the following order: pair1\_direct\_primer, pair1\_reverse\_primer, pair2\_direct\_primer, pair2\_reverse\_primer, etc. This could be a multifasta file, for example.

Second, the primers are checked for heterodimer formations. If there is no such formations between all primers in two or more primer pairs, it means that these pairs can be put simultaneously in the same reaction tube, so the workflow GROUPS these primer pairs.

However, please note that this workflow doesn't check the correctness of the primers themselves, for example for hairpins, selfdimers, etc.

The result report of the analysis is stored, by default, in the "report.html" file.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Group Primer Pairs" can be found in the "Scenarios" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930550/65930551.png)

##### Workflow Wizard

The wizard has 2 pages.

1.  Input primers: On this page you must input primers.


    ![](/images/65930550/65930552.png)

2.  Output report file: On this page you can modify output parameters.


    ![](/images/65930550/65930553.png)
