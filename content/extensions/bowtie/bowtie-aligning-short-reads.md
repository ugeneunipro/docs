---
title: "Bowtie Aligning Short Reads"
weight: 100
---


# Bowtie Aligning Short Reads

When you select the _Tools ‣ DNA Assembly ‣ Align short reads_ item in the main menu, the _Align Short Reads_ dialog appears. Set value of the _Align short reads method_ parameter to _Bowtie_. The dialog looks as follows:


![](/images/65930853/107020295.png)

There are the following parameters:

_Reference sequence_ — DNA sequence to align short reads to. This parameter is required.

_Result file name_ — file in SAM format to write the result of the alignment into. This parameter is required.

_Library_ - single-end or paired-end reads.

_Prebuilt index_ — check this box to use an index file instead of a source reference sequence. The index is a set of 6 files with suffixes .1.ebwt, .2.ebwt, .3.ebwt, .4.ebwt, .rev.1.ebwt, and .rev.2.ebwt. The index is created during the alignment. Also you can [_build it manually_](http://ugene.unipro.ru/documentation/manual/plugins/bowtie/build_index.html#bowtie-build-index).

_SAM output_ — always save the output file in the SAM format (the option is disabled for _Bowtie_).

_Short reads_ — each added short read is a small DNA sequence file. At least one read should be added.

Short reads length for _Bowtie_ can’t be more than 1024.

You can also configure other parameters. They are the same as in the original _Bowtie_ (you can read detailed description of the parameters on the [Bowtie manual page](http://bowtie-bio.sourceforge.net/manual.shtml)).

Select one of the following alignment modes:

The _\-n_ alignment mode:

When the _\-n mode_ is selected, _Bowtie_ determines which alignments are valid according to the following policy. Alignments may have no more than N mismatches (where N is a number 0-3) in the first L bases (where L is a number 5 or greater, set with _Seed length_) on the high-quality (left) end of the read. The sum of the Phred quality values at all mismatched positions (not just in the seed) may not exceed E (set with _Maq error_). Where qualities are unavailable (e.g. if the reads are from a FASTA file), the Phred quality defaults to 40.

The _\-v_ alignment mode:

In _\-v mode_, alignments may have no more than V mismatches, where V may be a number from 0 through 3. Quality values are ignored. The _\-v mode_ is mutually exclusive with the _\-n mode_.

The following parameters are available:

_Maq error (–maqerr)_ — maximum permitted total of quality values at all mismatched read positions throughout the entire alignment, not just in the “seed”. The default is 70. By default, _Bowtie_ rounds quality values to the nearest 10 and saturates at 30. Note that the rounding can be disabled with _No Maq rounding_.

_Seed Length (–seedlen)_ — the number of bases on the high-quality end of the read to which the _\-n_ applies. The lowest permitted setting is 5 and the default is 28.

_Maximum of backtracks (-maxbts)_ — the maximum number of backtracks (default: 125 without _Best_, 800 with _Best_). A “backtrack” is the introduction of a speculative substitution into the alignment.

_Descriptors memory usage (–chunkmbs)_ — the number of megabytes of memory a given thread is given to store path descriptors in the _Best_ flag. Default: 64. This parameter is available if the _Best_ flag is checked.

_Seed (–seed)_ — pseudo-random number generator.

The following flags are available:

_No Maq rounding (–nomaqround)_ — Maq (Mapping and Assembly with Quality) accepts quality values in the Phred quality scale, but internally rounds values to the nearest 10, with a maximum of 30. By default, _Bowtie_ also rounds this way. _No Maq rounding_ prevents this rounding in _Bowtie_.

_No forward orientation (–nofw)_ — do not attempt to align against the forward reference strand.

_No reverse-complement orientation (–norc)_ — do not attempt to align against the reverse-complement reference strand.

_Try as hard (–tryhard)_ — try as hard as possible to find valid alignments when they exist, including paired-end alignments.

_Best alignments (–best)_ — make _Bowtie_ guarantee that reported singleton alignments are “best” in terms of stratum (i.e. number of mismatches, or mismatches in the seed for the case of _\-n mode_) and in terms of the quality values at the mismatched position(s).

_All alignments (–all)_ — report all valid alignments per read or pair. Validity of alignments is determined by the alignment policy (combined effects of _\-n mode_, _\-v mode_, _Seed length_, and _Maq error_).

Select the required parameters and press the _Start_ button.
