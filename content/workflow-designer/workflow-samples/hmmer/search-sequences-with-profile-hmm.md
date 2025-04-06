---
title: "Search Sequences with Profile HMM"
weight: 1
---


# Search Sequences with Profile HMM

This workflow reads an HMM from a file and searches input sequences for significantly similar matches, saves found signals to a file. You can specify several input files for both HMM and sequences, the workflow will process Cartesian product of inputs. That is, each sequence will be searched with all specified HMMs in turn.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Search Sequences with Profile HMM" can be found in the "HMMER" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930309/65930310.png)

##### Workflow Wizard

The wizard has 2 pages.

1.  Input sequence(s): On this page you must input sequence(s).


    ![](/images/65930309/65930311.png)

2.  HMM search: On this page you can modify HMM search parameters.


    ![](/images/65930309/65930312.png)

    The following parameters are available:

    HMM profile(s)

    Semicolon-separated list of paths to the input files.

    Result annotation

    A name of the result annotations.

    Number of seqs

    Calculate the E-value scores as if we had seen a sequence database of sequences.

    Filter by high E-value

    E-value filtering can be used to exclude low-probability hits from result.

    Filter by low score

    Score based filtering is an alternative to E-value filtering to exclude low-probability hits from result.

    Result Genbank file

    Location of output data file. If this attribute is set, slot "Location" in port will not be used.

    Accumulate objects

    Accumulate all incoming data in one file or create separate files for each input.In the latter case, an incremental numerical suffix is added to the file name.
