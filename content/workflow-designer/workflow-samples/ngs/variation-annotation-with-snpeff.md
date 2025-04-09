---
title: "Variation Annotation with SnpEff"
weight: 1500
---


# Variation Annotation with SnpEff

SnpEff is a variant annotation and effect prediction tool. It annotates and predicts the effects of genetic variants (such as amino acid changes).

A typical SnpEff use case would be:
\-Input: The inputs are predicted variants (SNPs, insertions, deletions, and MNPs). The input file is usually obtained as a result of a sequencing experiment, and it is usually in variant call format (VCF).
\-Output: SnpEff analyzes the input variants. It annotates the variants and calculates the effects they produce on known genes (e.g. amino acid changes).

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Variation Annotation with SnpEff" can be found in the "NGS" section of the Workflow Designer samples.

##### Workflow Image

The opened workflow looks as follows:


![](/images/65930434/71958566.png)

##### Workflow Wizard

The wizard has 4 pages.

1.  Input Variations: On this page, you must input variations file(s).


    ![](/images/65930434/71958571.png)

2.  Change chromosome notation for variations: On this page you can change the chromosome notation for variations.


    ![](/images/65930434/65930436.png)

    The following parameters are available:

    Replace prefixes

    Input the list of chromosome prefixes that you would like to replace. For example "NC\_000". Separate different prefixes by semicolons.

    Replace by

    Input the prefix that should be set instead, for example "chr".

3.  SnpEff Parameters: On this page you can modify SnpEff parameters.


    ![](/images/65930434/65930437.png)

    The following parameters are available:

    Genome

    Select the target genome. Genome data will be downloaded if it is not found.

    Cannonical transcripts

    Use only cannonical transcripts

    HGVS nomenclature

    Annotate using HGVS nomenclature

    Annotate Loss of function

    Annotate Loss of function (LOF) and Nonsense mediated decay (NMD)



    Annotate TFBSs motifs

    Annotate transcription factor binding site motifs (only available for latest GRCh37)

    Upstream/downstream length

    Upstream and downstream interval size. Eliminate any upstream and downstream effect by using 0 length

4.  Output: On this page, you need input output parameters.


    ![](/images/65930434/65930438.png)
