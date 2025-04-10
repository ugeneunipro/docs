---
title: "Marking by Length"
weight: 200
---

# Marking by Length

This sample describes how to identify sequences with a specified length.

First, the workflow reads sequences inputted by a user. Then, each sequence is marked either as “Short” or “Long,” depending on the sequence's length. After marking, the sequences are filtered by these marks. Finally, the filtered sequences are written into files as specified by the user.

By default, a sequence with a length of 200 base pairs (bp) or less is marked as “Short.” A sequence longer than 200 bp is marked as “Long.” You can configure this value in the [_Sequence Marker_](../../workflow-elements/data-flow/sequence-marker-element) element parameters.

How to Use This Sample:

If you haven't used workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Marking Sequences by Length" can be found in the "Data Marking" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:

![](/images/65930283/65930284.png)