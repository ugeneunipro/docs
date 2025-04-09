---
title: "Quality Filter"
weight: 500
---


# Quality Filter

This workflow filters sequences with quality >= than parameter "quality" and writes result in file in FASTQ format.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Quality Filter" can be found in the "Custom Elements" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930275/65930276.png)

##### Workflow Wizard

The wizard has 2 pages.

1.  Input sequence(s): On this page you must input sequence(s).


    ![](/images/65930275/65930277.png)

2.  Quality Filter: On this page you can modify quality filter and output settings.


    ![](/images/65930275/65930278.png)

    The following parameters are available:

    Minimum quality value

    Minimum quality value

    Result FASTQ file

    Location of output data file. If this attribute is set, slot "Location" in port will not be used.

    Accumulate results

    Accumulate all incoming data in one file or create separate files for each input.In the latter case, an incremental numerical suffix is added to the file name.
