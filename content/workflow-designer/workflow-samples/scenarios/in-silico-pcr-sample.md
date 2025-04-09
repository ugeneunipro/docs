---
title: "In Silico PCR Sample"
weight: 900
---


# In Silico PCR Sample

This workflow simulates the PCR process.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "In Silico PCR" can be found in the "Scenarios" section of the Workflow Designer samples.

##### Workflow Image

The opened workflow looks as follows:


![](/images/65930567/76709919.png)

##### Workflow Wizard

The wizard has 3 pages.

1.  Input DNA Sequences: On this page you must input DNA sequences.


    ![](/images/65930567/65930568.png)

2.  Primers and Parameters: Here you must input _Primers_ and you can optionally modify _In Silico PCR_ parameters.


    ![](/images/65930567/65930569.png)

    The following parameters are available:

    Primers URL

    A URL to the input file with primer pairs.

    Mismatches

    Number of allowed mismatches.

    Min perfect match

    Number of bases that match exactly on 3' end of primers.

    Max product size

    Maximum size of amplified region.

    Use ambiguous bases

    Search for ambiguous bases (as "N") if checked.

    The input primers file should be in the FASTA format and contain an even number of primers (because each pair should have forward and reverse primers).

    Example format:
    \>forward
    CTTGTATGAATGGCCGCACG
    \>reverse
    GATGTAGCGGGTCGTAGTGG



3.  Output data: Here you can see information about output data.


    ![](/images/65930567/65930571.png)
