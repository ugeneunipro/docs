---
title: "Test for Diff. Expression with Cuffdiff Element"
weight: 1
---


# Test for Diff. Expression with Cuffdiff Element

Cuffdiff takes a transcript file as input, along with two or more fragment alignments (e.g. in SAM format) for two or more samples. It produces a number of output files that contain test results for changes in expression at the level of transcripts, primary transcripts, and genes. It also tracks changes in the relative abundance of transcripts sharing a common transcription start site, and in the relative abundances of the primary transcripts of each gene. Tracking the former allows one to see changes in splicing, and the latter lets one see changes in relative promoter use within a gene.

**Element type:** cuffdiff

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Directory to save MACS output files.



**out-dir**

_string_

**Time series analysis**

If set to True, instructs Cuffdiff to analyze the provided samples as a time series, rather than testing for differences between all pairs of samples. Samples should be provided in increasing time order.

False

**time-series-analysis**

_boolean_

**Upper quartile norm**

If set to True, normalizes by the upper quartile of the number of fragments mapping to individual loci instead of the total number of sequenced fragments. This can improve robustness of differential expression calls for less abundant genes and transcripts.

False

**upper-quartile-norm**

_boolean_

**Hits norm**

 Instructs how to count all fragments. Total specifies to count all fragments, including those not compatible with any reference transcript, towards the number of mapped fragments used in the FPKM denominator. Compatible specifies to use only compatible fragments. Selecting Compatible is generally recommended in Cuffdiff to reduce certain types of bias caused by differential amounts of ribosomal reads which can create the impression of falsely differentially expressed genes..

Compatible

**hits-norm**

_numeric_

**Frag bias correct**

Providing the sequences your reads were mapped to instructs Cuffdiff to run bias detection and correction algorithm which can significantly improve accuracy of transcript abundance estimates..



**frag-bias-correct**

_string_

**Multi read correct**

Do an initial estimation procedure to more accurately weight reads mapping to multiple locations in the genome.

False

**multi-read-correct**

_boolean_

**Library type**

Specifies RNA-Seq protocol.

Standard Illumina

**library-type**

_numeric_

**Mask file**

Ignore all reads that could have come from transcripts in this file. It is recommended to include any annotated rRNA, mitochondrial transcripts other abundant transcripts you wish to ignore in your analysis in this file. Due to variable efficiency of mRNA enrichment methods and rRNA depletion kits, masking these transcripts often improves the overall robustness of transcript abundance estimates..



**mask-file**

_numeric_

**Min alignment count**

The minimum number of alignments in a locus for needed to conduct significance testing on changes in that locus observed between samples. If no testing is performed, changes in the locus are deemed not significant, and the locus' observed changes don't contribute to correction for multiple testing..

10

**min-alignment-count**

_string_

**FDR**

The allowed false discovery rate used in testing.

0.05

**fdr**

_numeric_

**Max MLE iterations**

Sets the number of iterations allowed during maximum likelihood estimation of abundances.

5000

**max-mle-iterations**

_numeric_

**Emit count tables**

Include information about the fragment counts, fragment count variances, and fitted variance model into the report.

False

**emit-count-tables**

_boolean_

**Cuffdiff tool path**

The path to the Cuffdiff external tool in UGENE.

defaul

**path**

_string_

**Temporary directory**

The directory for temporary files.

default

**temp-dir**

_string_

Input/Output Ports
------------------

The element has 2 _input port_:

**Name in GUI:** Annotations

**Name in Workflow File:** in-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**in-annotations**

_ann\_table_

**Name in GUI:** Assembly

**Name in Workflow File:** in-assembly

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Assembly data**

**assembly**

_assembly_

**Source url**

**url**

_string_
