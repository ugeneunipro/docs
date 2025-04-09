---
title: "Building Index for UGENE Genome Aligner"
weight: 100
---


# Building Index for UGENE Genome Aligner

You can build an index to optimize short reads alignment using [_UGENE Genome Aligner_](ugene-genome-aligner.md). To open the _Build Index_ dialog, select the _Tools ‣ NGS data analysis ‣ Build index for reads mapping_ item in the main menu. Set value of the _Map short reads method_ parameter to _UGENE Genome Aligner_.

The dialog looks as follows:


![](/images/65930893/82608149.png)

The parameters are the following:

_Reference sequence_ — DNA sequence to which short reads would be aligned to. This parameter is required.

_Index file name_ — file to save index to. This parameter is required.

_Reference fragmentation_ — this parameter influences the amount of parts the reference will be divided. It is better to make it bigger, but it influences the amount of memory used during the alignment.

_Total memory usage_ — shows the total memory usage.

_System memory size_ — shows the total system memory size.
