---
title: "Convert seq-qual Pair to FASTQ"
weight: 100
---


# Convert seq-qual Pair to FASTQ

This workflow allows to add PHRED quality scores to the sequence and save output to Fastq. For example, one can read a Fasta file, import PHRED quality values from corresponding qualities file and export the result to Fastq.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Convert "seq/qual" Pair to FASTQ" can be found in the "Conversions" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930245/65930246.png)

##### Workflow Wizard

The wizard has 2 pages.

1.  Input Sequence(s): On this page you must input sequences(s).


    ![](/images/65930245/65930247.png)

2.  Convert "seq/qual" Pair to FASTQ: On this page you can modify converting and output settings.


    ![](/images/65930245/65930248.png)

    The following parameters are available:

    PHRED input

    Path to file with PHRED quality scores.

    Quality type

    Choose method to encode quality scores.

    File format

    Quality values can be in specialized FASTA-like PHRED qual format or encoded similar as in FASTQ files.

    Result file

    Location of output data file. If this attribute is set, slot "Location" in port will not be used.

    Accumulate results

    Accumulate all incoming data in one file or create separate files for each input.In the latter case, an incremental numerical suffix is added to the file name.
