---
title: "Variants Calling"
weight: 2800
---

# Variants Calling

**Task Name:** `snp`

Call variants for an input assembly and a reference sequence using SAMtools mpileup and bcftools.

**Parameters:**

- `bam` - Input sorted BAM file(s) [URL datasets]
- `ref` - Input reference sequence [URL datasets]
- `wout` - Output file with variations [String]
- `bN` - A/C/G/T only [Boolean]
- `bI` - List of sites [String]
- `ml` - BED or position list file [String]
- `bg` - Per-sample genotypes [Boolean]
- `mC` - Mapping quality downgrading coefficient [Number]
- `bT` - Pair/trio calling [String]
- `mB` - Disable BAQ computation [Boolean]
- `me` - Gap extension error [Number]
- `mE` - Extended BAQ computation [Boolean]
- `bF` - Indicate PL [Boolean]
- `vw` - Gap size [Number]
- `m6` - Illumina-1.3+ encoding [Boolean]
- `bi` - INDEL-to-SNP Ratio [Number]
- `bA` - Retain all possible alternates [Boolean]
- `vD` - Max number of reads per input BAM [Number]
- `md` - Max number of reads per input BAM [Number]
- `mL` - Max INDEL depth [Number]
- `va` - Alternate bases [Number]
- `v2` - BaseQ bias [String]
- `vd` - Minimum read depth [Number]
- `v4` - End distance bias [Number]
- `v3` - MapQ bias [Number]
- `Q` - Minimum RMS quality [Number]
- `v1` - Strand bias [Number]
- `mQ` - Minimum base quality [Number]
- `mq` - Minimum mapping quality [Number]
- `bd` - Min samples fraction [Number]
- `b1` - N group-1 samples [Number]
- `bU` - N permutations [Number]
- `bG` - No genotype information [Boolean]
- `mI` - No INDELs [Boolean]
- `mo` - Gap open error [Number]
- `mP` - List of platforms for indels [String]
- `vp` - Log filtered [Boolean]
- `bP` - Prior allele frequency spectrum [String]
- `bQ` - QCALL likelihood [Boolean]
- `mr` - Pileup region [String]
- `bs` - List of samples [String]
- `mh` - Homopolymer errors coefficient [Number]
- `bt` - Mutation rate [Number]
- `mA` - Count anomalous read pairs [Boolean]
- `vW` - A/C/G/T only [Number]

**Example:**

```
ugene snp --bam=test.bam --ref=test_ref.fa --wout=test_out.vcf