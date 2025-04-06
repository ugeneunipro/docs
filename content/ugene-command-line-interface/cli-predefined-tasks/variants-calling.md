---
title: "Variants Calling"
weight: 1
---


# Variants Calling

**Task Name:** snp

Call variants for an input assembly and a reference sequence using SAMtools mpileup and bcftool

**Parameters:**

_bam_ - Input sorted BAM file(s) \[Url datasets\]

_ref_ - Input reference sequence \[Url datasets\]

_wout_ - Out file with variations \[String\]

_bN_ - A/C/G/T only \[Boolean\]

_bI_ - List of sites \[String\]

_ml_ - BED or position list file \[String\]

_bg_ - Per-sample genotypes \[Boolean\]

_mC_ - Mapping quality downgrading coefficient \[Number\]

_bT_ - Pair/trio calling \[String\]

_mB_ - Disable BAQ computation \[Boolean\]

_me_ - Gap extension error \[Number\]

_mE_ - Extended BAQ computation \[Boolean\]

_bF_ - Indicate PL \[Boolean\]

_vw_ - Gap size \[Number\]

_m6_ - Illumina-1.3+ encoding \[Boolean\]

_bi_ - INDEL-to-SNP Ratio \[Number\]

_bA_ - Retain all possible alternate \[Boolean\]

_vD_ - Max number of reads per input BAM \[Number\]

_md_ - Max number of reads per input BAM \[Number\]

_mL_ - Max INDEL depth \[Number\]

_va_ - Alternate bases \[Number\]

_v2_ - BaseQ bias \[String\]

_vd_ - Minimum read depth \[Number\]

_v4_ - End distance bias \[Number\]

_v3_ - MapQ bias \[Number\]

_Q_ - Minimum RMS quality \[Number\]

 _v1_ - Strand bias \[Number\]

 _mQ_ - Minimum base quality \[Number\]

 _mq_ - Minimum mapping quality \[Number\]

 _bd_ - Min samples fraction \[Number\]

 _b1_ - N group-1 samples \[Number\]

 _bU_ - N permutations \[Number\]

 _bG_ - No genotype information \[Boolean\]

 _mI_ - No INDELs \[Boolean\]

 _mo_ - Gap open error \[Number\]

 _mP_ - List of platforms for indels \[String\]

 _vp_ - Log filtered \[Boolean\]

 _bP_ - Prior allele frequency spectrum. \[String\]

 _bQ_ - QCALL likelihood \[Boolean\]

 _mr_ - Pileup region \[String\]

 _bs_ - List of samples \[String\]

 _mh_ - Homopolymer errors coefficient \[Number\]

 _bt_ - Mutation rate \[Number\]

 _mA_ - Count anomalous read pairs \[Boolean\]

 _vW_ - A/C/G/T only \[Number\]

**Example:**

ugene snp --bam=test.bam --ref=test\_ref.fa --wout=test\_out.vcf
