---
title: "Aligning Short Reads with BWA"
weight: 1
---


# Aligning Short Reads with BWA

When you select the _Tools ‣ DNA Assembly ‣ Align short reads_ item in the main menu, the _Align Short Reads_ dialog appears. Set value of the _Align short reads method_ parameter to _BWA_. The dialog looks as follows:


![](/images/65930870/65930871.png)

There are the following parameters:

_Reference sequence_ — DNA sequence to align short reads to. This parameter is required.

_Result file name_ — file in SAM format to write the result of the alignment into. This parameter is required.

_Library_ - single-end or paired-end reads.

_Prebuilt index_ — check this box to use an index file instead of a source reference sequence. Also you can [_build it manually_](http://ugene.unipro.ru/documentation/manual/plugins/bwa/build_index.html#bwa-build-index).

_SAM output_ — always save the output file in the SAM format (the option is disabled for _BWA_).

_Short reads_ — each added short read is a small DNA sequence file. At least one read should be added.

You can also configure other parameters. They are the same as in the original _BWA_ (you can read detailed description of the parameters on the [BWA manual page](http://bio-bwa.sourceforge.net/)). Select one of the following parameters, that correspond to the _\-n_ option in the original _BWA_.

_Max #diff (-n)_ — maximum edit distance. An integer value should be input.

_Missing prob (-n)_ — the fraction of missing alignments given 2% uniform base error rate. A float value is used.

_Seed length (-l)_ — take the subsequence of the specified length as seed. If the specified length is larger than the query sequence, seeding will be disabled. For long reads, this option is typically ranged from 25 to 35.

_Max gap opens (-o)_ — maximum number of gap opens.

_Index algorithm (-a)_ — algorithm for constructing BWA index.

It implements three different algorithms:

*   *   _is_ — designed for short reads up to ~200bp with low error rate (<3%). It does gapped global alignment w.r.t. reads, supports paired-end reads, and is one of the fastest short read alignment algorithms to date while also visiting suboptimal hits.
    *   _bwtsw_ — is designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. Algorithm implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_. is slower and less accurate than the _is_ algorithm, but on long reads, it is better.
    *   _div_ — does not work for long genomes.

__Best hits (-R)_ — proceed with suboptimal alignments if there are no more than specified number of equally best hits. This option only affects paired-end mapping. Increasing this threshold helps to improve the pairing accuracy at the cost of speed, especially for short reads (~32bp)._

_Long-scaled gap penalty for long deletion (-L)_ — long-scaled gap penalty for long deletion.

_Non-iterative mode (-N)_ — disable iterative search. All hits with no more than _Max #diff_ differences will be found. This mode is much slower than the default.

You can also configure the following advanced parameters:

_Enable long gaps_ — checking this box allows one to set the _Max gap extentions_ parameter.

_Max gap extensions (-e)_ — maximum number of gap extensions.

_Indel offset (-i)_ — disallow insertions and deletions within the specified number of base pairs towards the ends.

_Max long deletion extensions (-d)_ — disallow a long deletions within the specified number of base pairs towards the 3\`-end.

_Max queue entries (-m)_ — maximum queue entries.

_Barcode length (-B)_ — length of barcode starting from the 5\`-end. When the specified length is positive, the barcode of each read will be trimmed before mapping and will be written at the BC SAM tag. For paired-end reads, the barcode from both ends are concatenated.

__Threads (-t)_ — number of threads._

_Max seed differences (-k)_ — maximum edit distance in the seed.

_Mismatch penalty (-M)_ — _BWA_ will not search for suboptimal hits with a score lower than the specified value.

_Gap open penalty (-O)_ — gap open penalty.

_Gap extension penalty (-E)_ — gap extension penalty.

_Quality threshold (-q)_ — parameter for read trimming.

Select the required parameters and press the _Start_ button.
