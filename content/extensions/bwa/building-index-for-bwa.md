---
title: "Building Index for BWA"
weight: 1
---


# Building Index for BWA

To build _BWA_ index select the _Tools ‣ NGS data analysis ‣ Build index for reads mapping_ item in the main menu. The _Build Index_ dialog appears. Set the _Map short reads method_ parameter to _BWA_.

The dialog looks as follows:


![](/images/65930872/88080408.png)

There are the following parameters:

_Reference sequence_ — DNA sequence to which short reads would be aligned to. This parameter is required.

_Index file name_ — file to save index to. This parameter is required.

_Index algorithm (-a)_ — Algorithm for constructing BWA index. Available options are:

It implements three different algorithms

*   *   _is_ — designed for short reads up to ~200bp with low error rate (<3%). It does gapped global alignment w.r.t. reads, supports paired-end reads, and is one of the fastest short read alignment algorithms to date while also visiting suboptimal hits.
    *   _bwtsw_ — is designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. Algorithm implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_. is slower and less accurate than the _is_ algorithm, but on long reads, it is better.
    *   _div_ — does not work for long genomes.

The value _"autodetect"_ by default means that the index (one of three) is chosen automatically depending on the length of the sequence.
