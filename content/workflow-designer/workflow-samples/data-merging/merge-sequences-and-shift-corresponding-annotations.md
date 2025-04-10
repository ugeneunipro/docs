---
title: "Merge Sequences and Shift Corresponding Annotations"
weight: 200
---


# Merge Sequences and Shift Corresponding Annotations

This workflow describes how to merge sequences and handle their annotations.

First, the workflow reads sequence(s) from file(s). Then, it marks the input sequences with the sequence name marker. After marking, the sequences are grouped by the marker. Sequences with equal markers are merged into one sequence. Annotations are shifted based on the position of the corresponding sequence within the merged sequence. Finally, the grouped data are written into a file specified by the user.

By default, a sequence is marked using the sequence name marker. You can configure this value in the [_Marker_](../../workflow-elements/data-flow/sequence-marker-element) element parameters. Also, you can configure the [_Grouper_](../../workflow-elements/data-flow/grouper-element) element parameters.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Merge Sequences and Shift Corresponding Annotations" can be found in the "Data Merging" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930293/65930294.png)