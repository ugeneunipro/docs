---
title: "Bowtie 2 Aligning Short Reads"
weight: 100
---

# Bowtie 2: Aligning Short Reads

When you select the _Tools ‣ Align to reference ‣ Align short reads_ item in the main menu, the _Align Sequencing Reads_ dialog appears. Set the value of the _Align short reads method_ parameter to _Bowtie 2_. The dialog looks as follows:

![](/images/65930862/65930863.png)

There are the following parameters:

_Reference sequence_ — DNA sequence to align short reads to. This parameter is required.

_Result file name_ — file in SAM format to write the result of the alignment into. This parameter is required.

_Library_ — single-end or paired-end reads.

_Prebuilt index_ — check this box to use an index file instead of a source reference sequence. The index is a set of 6 files with suffixes .1.ebwt, .2.ebwt, .3.ebwt, .4.ebwt, .rev.1.ebwt, and .rev.2.ebwt. The index is created during the alignment. You can also [_build it manually_](http://ugene.unipro.ru/documentation/manual/plugins/bowtie/build_index.html#bowtie-build-index).

_SAM output_ — always save the output file in the SAM format (this option is disabled for _Bowtie_).

_Short reads_ — each added short read is a small DNA sequence file. At least one read should be added.

You can also configure other parameters. They are the same as in the original _Bowtie 2_ (you can read a detailed description of the parameters on the [Bowtie 2 manual page](http://bowtie-bio.sourceforge.net/bowtie2/index.shtml)).

Select one of the following alignment modes:

- The --end-to-end alignment mode:  
By default, Bowtie 2 performs end-to-end read alignment. That is, it searches for alignments involving all of the read characters. This is also called an "untrimmed" or "unclipped" alignment.

- When the --local option is specified:  
Bowtie 2 performs local read alignment. In this mode, Bowtie 2 might "trim" or "clip" some read characters from one or both ends of the alignment if doing so maximizes the alignment score.

The following parameters are available:

_Number of mismatches (--N)_ — sets the number of mismatches allowed in a seed alignment during multiseed alignment. Can be set to 0 or 1. Setting this higher makes alignment slower (often much slower) but increases sensitivity.

_Seed length (–L)_ — sets the length of the seed substrings to align during multiseed alignment. Smaller values make alignment slower but more sensitive.

_Add columns to allow gaps (--dpad)_ — "pads" dynamic programming problems by `<int>` columns on either side to allow gaps.

_Disallow gaps (–gbar)_ — disallow gaps within `<int>` positions of the beginning or end of the read.

_Seed (–seed)_ — use `<int>` as the seed for the pseudo-random number generator.

The following flags are available:

_No unpaired alignments (–no-mixed)_ — by default, when `bowtie2` cannot find a concordant or discordant alignment for a pair, it then tries to find alignments for the individual mates. This option disables that behavior.

_No discordant alignments (–no-discordant)_ — by default, `bowtie2` looks for discordant alignments if it cannot find any concordant alignments. A discordant alignment is an alignment where both mates align uniquely, but that does not satisfy the paired-end constraints. This option disables that behavior.

_No forward orientation (–nofw)_ — if `--nofw` is specified, `bowtie2` will not attempt to align unpaired reads to the forward (Watson) reference strand.

_No reverse-complement orientation (–norc)_ — if `--norc` is specified, `bowtie2` will not attempt to align unpaired reads against the reverse-complement (Crick) reference strand.

_No overlapping mates (–no-overlap)_ — if one mate alignment overlaps the other at all, it is considered non-concordant.

_No mates containing one another (–no-contain)_ — if one mate alignment contains the other, it is considered non-concordant.

Select the required parameters and press the _Start_ button.