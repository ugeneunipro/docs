---
title: "Call Variants with SAMtools Element"
weight: 100
---

# Call Variants with SAMtools Element

Calls SNPs and INDELS with SAMtools mpileup and bcftools.

**Element type:** call_variants

## Parameters

| Parameter                         | Description                                                                                       | Default value                                                                 | Parameter in Workflow File | Type      |
|-----------------------------------|---------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|----------------------------|-----------|
| **Output variants file**          | The URL to the file with the extracted variations.                                                |                                                                               |                            |           |
| **Reference**                     | File with the reference sequence for all NGS assemblies.                                          |                                                                               |                            | _string_  |
| **Use reference from**            | `File` (use same reference for all inputs) or `Input port` (different references via input port). | File                                                                          |                            | _string_  |
| **Illumina-1.3+ encoding**        | Assume Illumina 1.3+ quality encoding (mpileup `-6`).                                             | False                                                                         | **illumina13-encoding**    | _boolean_ |
| **Count anomalous read pairs**    | Do not skip anomalous read pairs (mpileup `-A`).                                                  | False                                                                         | **use_orphan**             | _boolean_ |
| **Disable BAQ computation**       | Disable base alignment quality calculation (mpileup `-B`).                                        | False                                                                         | **disable_baq**            | _boolean_ |
| **Mapping quality downgrade**     | Downgrade mapping quality for mismatched reads (mpileup `-C`). Recommended for BWA: 50.           | 0                                                                             | **capq_thres**             | _numeric_ |
| **Max reads per BAM**             | Limit number of reads per position (mpileup `-d`).                                                | 250                                                                           | **max_depth**              | _numeric_ |
| **Extended BAQ computation**      | Improves MNP sensitivity (mpileup `-E`).                                                          | False                                                                         | **ext_baq**                | _boolean_ |
| **BED or position list file**     | Regions to generate pileup for (mpileup `-l`).                                                    |                                                                               | **bed**                    | _string_  |
| **Pileup region**                 | Region to generate pileup (mpileup `-r`).                                                         |                                                                               | **reg**                    | _string_  |
| **Minimum mapping quality**       | Minimum mapping quality for alignments (mpileup `-q`).                                            | 0                                                                             | **min_mq**                 | _numeric_ |
| **Minimum base quality**          | Minimum base quality (mpileup `-Q`).                                                              | 13                                                                            | **min_baseq**              | _numeric_ |
| **Gap extension error**           | Error probability for gap extension (mpileup `-e`).                                               | 20                                                                            | **extQ**                   | _numeric_ |
| **Homopolymer error coefficient** | Error model coefficient for indels in homopolymers (mpileup `-h`).                                | 100                                                                           | **tandemQ**                | _numeric_ |
| **No INDELs**                     | Do not call INDELs (mpileup `-I`).                                                                | False                                                                         | **no_indel**               | _boolean_ |
| **Max INDEL depth**               | Skip INDELs above per-sample depth (mpileup `-L`).                                                | 250                                                                           | **max_indel_depth**        | _numeric_ |
| **Gap open error**                | Gap open error probability (mpileup `-o`).                                                        | 40                                                                            | **openQ**                  | _numeric_ |
| **Platform list for indels**      | Comma-separated list of platforms for indels (mpileup `-P`).                                      |                                                                               | **pl_list**                | _string_  |
| **Retain all alternates**         | Keep all alternate alleles (bcftools view `-A`).                                                  | False                                                                         | **keepalt**                | _boolean_ |
| **Indicate PL**                   | PL from older SAMtools versions (bcftools view `-F`).                                             | False                                                                         | **fix_pl**                 | _boolean_ |
| **No genotype information**       | Suppress genotypes (bcftools view `-G`).                                                          | False                                                                         | **no_geno**                | _boolean_ |
| **A/C/G/T only**                  | Skip sites where REF is not A/C/G/T (bcftools view `-N`).                                         | False                                                                         | **acgt_only**              | _boolean_ |
| **List of sites**                 | Limit to listed sites (bcftools view `-l`).                                                       |                                                                               | **bcf_bed**                | _string_  |
| **QCALL likelihood**              | Output QCALL format (bcftools view `-Q`).                                                         | False                                                                         | **qcall**                  | _boolean_ |
| **Sample list**                   | File with sample names and ploidy (bcftools view `-s`).                                           |                                                                               | **samples**                | _string_  |
| **Min sample fraction**           | Skip loci if < fraction of samples are covered (bcftools view `-d`).                              | 0                                                                             | **min_smpl_frac**          | _numeric_ |
| **Per-sample genotypes**          | Call genotypes (bcftools view `-g`).                                                              | True                                                                          | **call_gt**                | _boolean_ |
| **INDEL-to-SNP ratio**            | Expected mutation ratio (bcftools view `-i`).                                                     | -1                                                                            | **indel_frac**             | _numeric_ |
| **Max P(ref | D)**               | Site considered variant if probability of reference is below (bcftools view).                      | 0.5                                                                           | **pref**                   | _numeric_ |
| **Allele frequency prior**        | Allele frequency prior: `full`, `cond2`, `flat`, or previous run output (bcftools view `-P`).     | full                                                                          | **ptype**                  | _string_  |
| **Mutation rate**                 | Mutation rate (bcftools view `-t`).                                                               | 0.001                                                                         | **theta**                  | _numeric_ |
| **Pair/trio calling**             | Enable pair/trio calling (bcftools view `-T`).                                                    |                                                                               | **ccall**                  | _string_  |
| **N group-1 samples**             | Number of group-1 samples for association test (bcftools view `-1`).                              | 0                                                                             | **n1**                     | _numeric_ |
| **N permutations**                | Permutations for association test (bcftools view `-U`).                                           | 0                                                                             | **n_perm**                 | _numeric_ |
| **Min P(chi²)**                   | Threshold for P(chi²) to perform permutations.                                                    | 0.01                                                                          | **min_perm_p**             | _numeric_ |
| **Min RMS quality**               | Minimum RMS mapping quality for SNPs (varFilter `-Q`).                                            | 10                                                                            | **min-qual**               | _numeric_ |
| **Min read depth**                | Minimum read depth (varFilter `-d`).                                                              | 2                                                                             | **min-dep**                | _numeric_ |
| **Max read depth**                | Maximum read depth (varFilter `-D`).                                                              | 10000000                                                                      | **max-dep**                | _numeric_ |
| **Alternate bases**               | Minimum alternate base count (varFilter `-a`).                                                    | 2                                                                             | **min-alt-bases**          | _numeric_ |
| **Gap size**                      | SNPs within this distance of a gap are filtered (varFilter `-w`).                                 | 3                                                                             | **gap-size**               | _numeric_ |
| **Window size**                   | Filtering window for adjacent gaps (varFilter `-W`).                                              | 10                                                                            | **window**                 | _numeric_ |
| **Strand bias**                   | P-value threshold for strand bias (varFilter `-1`).                                               | 0.0001                                                                        | **min-strand**             | _numeric_ |
| **BaseQ bias**                    | Minimum P-value for baseQ bias (varFilter `-2`).                                                  | 1e-100                                                                        | **min-baseQ**              | _string_  |
| **MapQ bias**                     | Minimum P-value for mapping quality bias (varFilter `-3`).                                        | 0                                                                             | **min-mapQ**               | _numeric_ |
| **End distance bias**             | Minimum P-value for bias near sequence ends (varFilter `-4`).                                     | 0.0001                                                                        | **min-end-distance**       | _numeric_ |
| **HWE**                           | Minimum P-value for Hardy-Weinberg Equilibrium + F<0 (varFilter `-e`).                            | 0.0001                                                                        | **min-hwe**                | _numeric_ |
| **Log filtered**                  | Print filtered variants to log (varFilter `-p`).                                                  | False                                                                         | **print-filtered**         | _boolean_ |

## Input/Output Ports

The element has 2 _input ports_:

**Name in GUI:** Input assembly  
**Name in Workflow File:** in-assembly

| Slot In GUI      | Slot in Workflow File | Type     |
|------------------|-----------------------|----------|
| **Dataset name** | **dataset**           | _string_ |
| **Source url**   | **url**               | _string_ |

**Name in GUI:** Input sequences  
**Name in Workflow File:** in-sequence

| Slot In GUI    | Slot in Workflow File | Type     |
|----------------|-----------------------|----------|
| **Source url** | **url**               | _string_ |

And 1 _output port_:

**Name in GUI:** Output variations  
**Name in Workflow File:** out-variations

| Slot In GUI         | Slot in Workflow File | Type        |
|---------------------|-----------------------|-------------|
| **Variation track** | **variation-track**   | _variation_ |