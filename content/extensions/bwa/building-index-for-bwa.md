---
title: "Building Index for BWA"
weight: 200
---

# Building Index for BWA

To build the _BWA_ index, select the _Tools ‣ NGS data analysis ‣ Build index for reads mapping_ item in the main menu. The _Build Index_ dialog will appear. Set the _Map short reads method_ parameter to _BWA_.

The dialog looks as follows:

![](/images/65930872/88080408.png)

The parameters are as follows:

- _Reference sequence_ — the DNA sequence to which short reads will be aligned. This parameter is required.

- _Index file name_ — the file in which to save the index. This parameter is required.

- _Index algorithm (-a)_ — the algorithm for constructing the BWA index. Available options are:

  - _is_ — designed for short reads up to ~200bp with a low error rate (<3%). It performs gapped global alignment with respect to reads, supports paired-end reads, and is one of the fastest short-read alignment algorithms to date while also visiting suboptimal hits.

  - _bwtsw_ — designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. Algorithm implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_ is slower and less accurate than the _is_ algorithm, but on long reads, it is better.

  - _div_ — does not work for long genomes.

The default value _"autodetect"_ means that the index (one of three) is chosen automatically depending on the length of the sequence.