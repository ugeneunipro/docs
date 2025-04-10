---
title: "Aligning Short Reads with BWA-SW"
weight: 100
---

# Aligning Short Reads with BWA-SW

When you select the _Tools ‣ Align to reference ‣ Align short reads_ option in the main menu, the _Align Sequencing Reads_ dialog box will appear. Set the value of the _Align short reads method_ parameter to _BWA-SW_. The dialog box looks as follows:

![](/images/65930877/65930878.png)

The following parameters are available:

_Reference sequence_ — The DNA sequence to align short reads to. This parameter is required.

_Result file name_ — The file in SAM format to write the result of the alignment into. This parameter is required.

_SAM output_ — Always save the output file in the SAM format (this option is disabled for _BWA_).

_Short reads_ — Each added short read is a small DNA sequence file. At least one read should be added.

You can also configure other parameters:

_Index algorithm (-a)_ — The algorithm for constructing the BWA-SW index. It implements three different algorithms:

- _is_ — Designed for short reads up to ~200bp with a low error rate (<3%). It performs gapped global alignment with respect to reads, supports paired-end reads, and is one of the fastest short read alignment algorithms to date while also visiting suboptimal hits.
- _bwtsw_ — Designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. The algorithm is implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_ is slower and less accurate than the _is_ algorithm, but on long reads, it is better.
- _div_ — Not suitable for long genomes.

_Score for a match (-a)_ — The score of a match.

_Mismatch penalty (-b)_ — The mismatch penalty.

_Gap open penalty (-q)_ — The gap open penalty.

_Gap extension penalty (-r)_ — The gap extension penalty. The penalty for a contiguous gap of size k is q+k\*r.

_Band width (-w)_ — The band width in the banded alignment.

_Number of threads (-t)_ — The number of threads in multi-threading mode.

_Size of chunk of reads (-s)_ — The maximum SA interval size for initiating a seed. A higher -s increases accuracy at the cost of speed.

_Score threshold (divided by match score) (-T)_ — The minimum score threshold.

_Z-best (-z)_ — Z-best heuristics. A higher -z increases accuracy at the cost of speed.

_Number of seeds to start reverse alignment (-N)_ — The minimum number of seeds supporting the resultant alignment to skip reverse alignment.

_Mask level (-c)_ — Coefficient for threshold adjustment according to query length. Given an l-long query, the threshold for a hit to be retained is a\*max{T,c\*log(l)}.

_Prefer hard clipping in SAM output (-H)_ — Use hard clipping in the SAM output. This option may dramatically reduce redundancy in the output when mapping long contig or BAC sequences.

Select the required parameters and press the _Start_ button.