---
title: "Marking by Annotation Number"
weight: 100
---


# Marking by Annotation Number

This sample describes how to identify sequences with the specified number of annotations.

First, the schema reads sequences input by a user. Then, each sequence is marked either with the "Good" or with the "Rest" mark, depending on the number of the sequence annotations. After marking, the sequences are filtered by the marks. And finally, the filtered sequences are written into files, specified by a user.

By default, a sequence with 1 or more annotations is marked as "Good". You can configure this value in the _Sequence Marker_ element parameters. Also, it is possible to set up the annotation names that should be taken into account.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Marking Sequences by Annotation Number" can be found in the "Data Marking" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930280/65930281.png)
