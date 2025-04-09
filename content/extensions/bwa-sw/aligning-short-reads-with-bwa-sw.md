---
title: "Aligning Short Reads with BWA-SW"
weight: 100
---


# Aligning Short Reads with BWA-SW

When you select the _Tools ‣ Align to reference ‣ Align short reads_ item in the main menu, the _Align Sequencing Reads_ dialog appears. Set value of the _Align short reads method_ parameter to _BWA-SW_. The dialog looks as follows:


![](/images/65930877/65930878.png)

There are the following parameters:

_Reference sequence_ — DNA sequence to align short reads to. This parameter is required.

_Result file name_ — file in SAM format to write the result of the alignment into. This parameter is required.

_SAM output_ — always save the output file in the SAM format (the option is disabled for _BWA_).

_Short reads_ — each added short read is a small DNA sequence file. At least one read should be added.

You can also configure other parameters.

_Index algorithm (-a)_ — algorithm for constructing BWA-SW index.

It implements three different algorithms:

*   *   _is_ — designed for short reads up to ~200bp with low error rate (<3%). It does gapped global alignment w.r.t. reads, supports paired-end reads, and is one of the fastest short read alignment algorithms to date while also visiting suboptimal hits.
    *   _bwtsw_ — is designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. Algorithm implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_. is slower and less accurate than the _is_ algorithm, but on long reads, it is better.
    *   _div_ — does not work for long genomes.

_Score for a match_ _(-a)_ — score of a match.

_Mismatch penalty_ _(-b)_ — mismatch penalty.

_Gap open penalty (-q)_ — gap open penalty.

_Gap extention penalty (-r)_ — Gap extension penalty. The penalty for a contiguous gap of size k is q+k\*r.

_Band width (-w)_ - Band width in the banded alignment.

_Number of threads (-t)_ - Number of threads in the multi-threading mode.

_Size of chunk of reads (-s)_ - Maximum SA interval size for initiating a seed. Higher -s increases accuracy at the cost of speed.

_Score threshold (divided by much score) (-T)_ - minimum score threshold.

_Z-best (-z)_ - Z-best heuristics. Higher -z increases accuracy at the cost of speed.

_Number of seeds to start rev alignment (-N)_ - Minimum number of seeds supporting the resultant alignment to skip reverse alignment.

_Mask level (-c)_ - Coefficient for threshold adjustment according to query length. Given an l-long query, the threshold for a hit to be retained is a\*max{T,c\*log(l)}.

_Prefer hard clipping in SAM output (-H)_ - use hard clipping in the SAM output. This option may dramatically reduce the redundancy of output when mapping long contig or BAC sequences.

Select the required parameters and press the _Start_ button.
