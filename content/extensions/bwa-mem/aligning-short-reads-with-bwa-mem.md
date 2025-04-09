---
title: "Aligning Short Reads with BWA-MEM"
weight: 100
---


# Aligning Short Reads with BWA-MEM

When you select the _Tools ‣ Align to reference ‣ Align short reads_ item in the main menu, the _Align Sequencing Reads_ dialog appears. Set value of the _Align short reads method_ parameter to _BWA-MEM_. The dialog looks as follows:


![](/images/65930884/65930885.png)

There are the following parameters:

_Reference sequence_ — DNA sequence to align short reads to. This parameter is required.

_Result file name_ — file in SAM format to write the result of the alignment into. This parameter is required.

_Prebuilt index_ — check this box to use an index file instead of a source reference sequence. Also you can [_build it manually_](http://ugene.unipro.ru/documentation/manual/plugins/bwa/build_index.html#bwa-build-index).

_SAM output_ — always save the output file in the SAM format (the option is disabled for _BWA_).

_Short reads_ — each added short read is a small DNA sequence file. At least one read should be added.

You can also configure other parameters.

_Index algorithm (-a)_ — algorithm for constructing BWA index.

It implements three different algorithms:

*   *   _is_ — designed for short reads up to ~200bp with low error rate (<3%). It does gapped global alignment w.r.t. reads, supports paired-end reads, and is one of the fastest short read alignment algorithms to date while also visiting suboptimal hits.
    *   _bwtsw_ — is designed for long reads with more errors. It performs heuristic Smith-Waterman-like alignment to find high-scoring local hits. Algorithm implemented in [BWA-SW](http://seqanswers.com/wiki/BWA-SW). On low-error short queries, _BWA-SW_. is slower and less accurate than the _is_ algorithm, but on long reads, it is better.
    *   _div_ — does not work for long genomes.

_Number of threads_ _(-t)_ — number of threads.

_Min seed length_ _(-k)_ — minimum seed length. Matches shorter than _INT_ will be missed. The alignment speed is usually insensitive to this value unless it significantly deviates 20.

_Band width (-w)_ — band width. Essentially, gaps longer than _INT_ will not be found. Note that the maximum gap length is also affected by the scoring matrix and the hit length, not solely determined by this option.

_Dropoff (-d)_ — off-diagonal X-dropoff (Z-dropoff). Stop extension when the difference between the best and the current extension score is above |_i_\-_j_|\*_A_+_INT_, where _i_ and _j_ are the current positions of the query and reference, respectively, and _A_ is the matching score. Z-dropoff is similar to BLAST’s X-dropoff except that it doesn’t penalize gaps in one of the sequences in the alignment. Z-dropoff not only avoids unnecessary extension, but also reduces poor alignments inside a long good alignment.

_Internall seeds length (-r)_ - trigger re-seeding for a MEM longer than _minSeedLen_\*_FLOAT_. This is a key heuristic parameter for tuning the performance. Larger value yields fewer seeds, which leads to faster alignment speed but lower accuracy.

_Skip seeds threshold (-c)_ - discard a MEM if it has more than _INT_ occurence in the genome. This is an insensitive parameter.

_Drop chain threshold (-D)_ - drop chains shorter than FLOAT fraction of the longest overlapping chain.

_Rounds of mate rescues (-m)_ - perform at most INT rounds of mate rescues for each read.

_Skip mate rescue (-S)_ - skip mate rescue.

_Skip pairing (-P)_ - in the paired-end mode, perform SW to rescue missing hits only but do not try to find hits that fit a proper pair.

_Score for a match (-A)_ - matching score.

_Mismatch penalty (-B)_ - mismatch penalty. The sequence error rate is approximately: {.75 \* exp\[-log(4) \* B/A\]}.

_Gap open penalty (-O)_ - gap open penalty.

_Gap extention penalty (-E)_ - gap extension penalty. A gap of length k costs O + k\*E (i.e. _Gap open penalty_ is for opening a zero-length gap).

_Penalty for clipping (-L)_ - clipping penalty. When performing SW extension, BWA-MEM keeps track of the best score reaching the end of query. If this score is larger than the best SW score minus the clipping penalty, clipping will not be applied. Note that in this case, the SAM AS tag reports the best SW score; clipping penalty is not deducted.

_Penalty unpaired (-U)_ - penalty for an unpaired read pair. BWA-MEM scores an unpaired read pair as scoreRead1+scoreRead2-_INT_ and scores a paired as scoreRead1+scoreRead2-insertPenalty. It compares these two scores to determine whether we should force pairing.

_Score threshold (-T)_ - don’t output alignment with score lower than score threshold. This option only affects output.

Select the required parameters and press the _Start_ button.
