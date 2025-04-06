---
title: "Merge Sequences and Annotations"
weight: 1
---


# Merge Sequences and Annotations

This sample workflow shows how to merge input sequences with sets of annotations.

For example, you may have sequences in FASTA format and annotations in GFF format, and you would like to merge them and save the result into GenBank files.

The steps of the workflow are these:

1.  The workflow reads sequences from the input sequence files, e.g. _sequence1_, _sequence2_, _sequence3_.
2.  The workflow reads annotations from the input files with annotations, e.g. _ann\_set1_, _ann\_set2_, _ann\_set3_.
3.  The sequences and the annotations are multiplexed. The result is:
    *   _sequence1_ + _ann\_set1_
    *   _sequence2_ + _ann\_set2_
    *   _sequence3_ + _ann\_set3_
4.  The result is written to the output files.



How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Merge Sequences and Annotations" can be found in the "Scenarios" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930562/65930563.png)

##### Workflow Wizard

The wizard has 3 pages.

1.  Input sequence(s): On this page you must input sequence(s).


    ![](/images/65930562/65930564.png)

2.  Input annotation(s): On this page you must input annotation(s).


    ![](/images/65930562/65930565.png)

3.  Output data: On this page you can modify output parameters.


    ![](/images/65930562/65930566.png)
