---
title: "Merge Sequences and Shift Corresponding Annotations"
weight: 200
---


# Merge Sequences and Shift Corresponding Annotations

This workflow describes how to merge sequences and manipulate with its annotations.

First, the workflow reads sequence(s) from file(s). Then, marks the input sequences with the sequence name marker. After marking the sequences are grouped by the marker. Sequences with equal markers are merged into one sequence. Annotations are shifted using the position of the corresponding sequence at the merged sequence. And finally, the grouped data are written into file, specified by a user.

By default, sequence is marked using the sequence name marker. You can configure this value in the [_Marker_](sequence-marker-element.md) element parameters. Also, you can configure the [_Grouper_](grouper-element.md) element parameters.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Merge Sequences and Shift Corresponding Annotations" can be found in the "Data Merging" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930293/65930294.png)
