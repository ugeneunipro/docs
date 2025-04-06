---
title: "UGENE Command Line Interface"
weight: 1
---


# UGENE Command Line Interface

UGENE command line interface (CLI) was developed keeping in mind the following principles:

*   To make it as easy as popular shell commands.
*   To include all significant UGENE features.
*   To allow users to add their own commands.

To use UGENE CLI make sure to add the path to the UGENE executable to your **%PATH%** environment variable.

The general syntax is the following:

ugene \[\[--task=\]task\_name\] \[--task\_parameter=value ...\] \[-task\_parameter value ...\] \[--option\[=value\]\] \[-option\[ value\]\]

Here:

**task\_name** — task to execute, it can be one of the [_predefined tasks_](cli-predefined-tasks.md) or [_a task you have created_](creating-custom-cli-tasks.md).

**task\_parameter** — parameter of the specified task. Some parameters of a task are required, like _in_ and _out_ parameters of some tasks.

**option** — one of the [_CLI options_](cli-options.md).

See the example below:

ugene align --in=COI.aln -out result.aln -log-level-details

*   [CLI Options](cli-options.md)
*   [CLI Predefined Tasks](cli-predefined-tasks.md)
    *   [Format Converting Sequences](format-converting-sequences.md)
    *   [Converting MSA](converting-msa.md)
    *   [Extracting Sequence](extracting-sequence.md)
    *   [Finding ORFs](finding-orfs.md)
    *   [Finding Repeats](finding-repeats.md)
    *   [Finding Pattern Using Smith-Waterman Algorithm](finding-pattern-using-smith-waterman-algorithm.md)
    *   [Adding Phred Quality Scores to Sequence](adding-phred-quality-scores-to-sequence.md)
    *   [Local BLAST Search](local-blast-search.md)
    *   [Remote NCBI BLAST and CDD Requests](remote-ncbi-blast-and-cdd-requests.md)
    *   [Annotating Sequence with UQL Schema](annotating-sequence-with-uql-schema.md)
    *   [Building Profile HMM Using HMMER2](building-profile-hmm-using-hmmer2.md)
    *   [Searching HMM Signals Using HMMER2](searching-hmm-signals-using-hmmer2.md)
    *   [Aligning with MUSCLE](aligning-with-muscle.md)
    *   [Aligning with ClustalW](aligning-with-clustalw.md)
    *   [Aligning with ClustalO](aligning-with-clustalo.md)
    *   [Aligning with Kalign](aligning-with-kalign.md)
    *   [Aligning with MAFFT](aligning-with-mafft.md)
    *   [Aligning with T-Coffee](aligning-with-t-coffee.md)
    *   [Building PFM](building-pfm.md)
    *   [Searching for TFBS with PFM](searching-for-tfbs-with-pfm.md)
    *   [Building PWM](building-pwm.md)
    *   [Searching for TFBS with Weight Matrices](searching-for-tfbs-with-weight-matrices.md)
    *   [Building Statistical Profile for SITECON](building-statistical-profile-for-sitecon.md)
    *   [Searching for TFBS with SITECON](searching-for-tfbs-with-sitecon.md)
    *   [Fetching Sequence from Remote Database](fetching-sequence-from-remote-database.md)
    *   [Gene-by-Gene Report](gene-by-gene-report.md)
    *   [Reverse-Complement Converting Sequences](reverse-complement-converting-sequences.md)
    *   [Variants Calling](variants-calling.md)
    *   [Generating DNA Sequence](generating-dna-sequence.md)
*   [Creating Custom CLI Tasks](creating-custom-cli-tasks.md)


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
