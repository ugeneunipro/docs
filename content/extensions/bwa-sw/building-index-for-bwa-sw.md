---
title: "Building Index for BWA-SW"
weight: 200
---

# Building Index for BWA-SW

To build a _BWA-SW_ index, select the _Tools ‣ NGS data analysis ‣ Build index for reads mapping_ item in the main menu. The _Build Index_ dialog will appear. Set the _Map short reads method_ parameter to _BWA-SW_.

The dialog looks as follows:

![](/images/65930879/88080412.png)

The following parameters are available:

_Reference sequence_ — DNA sequence to which short reads will be aligned. This parameter is required.

_Index file name_ — File to save the index to. This parameter is required.

_Index algorithm (-a)_ — Algorithm for constructing the BWA index. Available options are:

| Algorithm | Description |
| --- | --- |
| _is_ | Designed for short reads up to ~200bp with a low error rate (<3%). It performs gapped global alignment with respect to reads, supports paired-end reads, and is one of the fastest short read alignment algorithms to date while also visiting suboptimal hits. |
| _bwtsw_ | Designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. The algorithm is implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_ is slower and less accurate than the _is_ algorithm, but for long reads, it is better. |
| _div_ | Does not work for long genomes. |

The default value _"autodetect"_ means that the index (one of the three) is chosen automatically depending on the length of the sequence.