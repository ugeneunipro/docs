---
title: "Trim and Map Sanger Reads"
weight: 1
---


# Trim and Map Sanger Reads

The workflow does the following things:

1) Reads a set of Sanger sequencing reads from ABI files.
2) Trims ends of the reads by the quality value.
3) Filter the short trimmed reads.
4) Maps the filtered trimmed reads to a reference sequence.

You can change the workflow parameters:

1) Quality threshold for the trimming.
2) Minimum read length. If length of a trimmed read is less than the minimum value than the read is filtered.

The output data are:

1) Multiple sequence alignment file. The first sequence of the alignment is the reference and other ones are the reads.
2) Annotated reference sequence file. The annotations are the mapped reads.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Trim and Map Sanger Reads" can be found in the "Sanger Sequencing" section of the Workflow Designer samples.

##### Workflow Image

The opened workflow looks as follows:


![](/images/65930523/65930524.png)

##### Workflow Wizard

The wizard has 4 pages.

1.  Reference Sequence: On this page you must input reference sequence.


    ![](/images/65930523/65930526.png)

2.  Input Sanger Reads (ABI Files): On this page you must input ABI file(s).


    ![](/images/65930523/65930528.png)

3.  Mapping Settings: On this page, you can modify mapping settings.


    ![](/images/65930523/66814012.png)

    The following parameters are available:

    Trimming quality threshold

    The quality threshold for trimming.

    Mapping min similarity

    Reads, whose similarity with the reference is less than the stated value, will be ignored.

    Read name in the resulting alignment

    Reads in the resulting alignment can be named either by the names of the sequences in the input files or by the input files names. For example, if the sequences have the same name, set this value to &quot; File name&quot; to be able to distinguish the reads in the resulting alignment.

4.  Results: On this page you can modify output files settings.


    ![](/images/65930523/66814014.png)
