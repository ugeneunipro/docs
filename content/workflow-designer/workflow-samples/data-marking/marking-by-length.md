---
title: "Marking by Length"
weight: 1
---


# Marking by Length

This sample describes how to identify sequences with the specified length.

First, the workflow reads sequences input by a user. Then, each sequence is marked either with the “Short” or with the “Long” mark, depending on the sequence length. After marking, the sequences are filtered by the marks. And finally, the filtered sequences are written into files, specified by a user.

By default, a sequence with a length 200 or less bp is marked as “Short”. A sequence with a length of more than 200 bp is marked as “Long”. You can configure this value in the [_Sequence Marker_](sequence-marker-element.md) element parameters.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Marking Sequences by Length" can be found in the "Data Marking" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930283/65930284.png)
