---
title: "Quality Control by FastQC"
weight: 600
---


# Quality Control by FastQC

FastQC aims to provide a simple way to do some quality control checks on raw sequence data coming from high througput sequencing pipelines. It provides a molecular set of analyses which you can use to give a quick impression of whether your data has any problems of which you should be aware before doing any further analysis.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Quality Control by FastQC" can be found in the "NGS" section of the Workflow Designer samples.

##### Workflow Image

The workflow is the following:


![](/images/65930352/65930353.png)

##### Workflow Wizard

The wizard has 1 page.

1.  High Throughput Sequence QC Report by FastQC: On this page you must input FASTQ file(s) and optionally modify advanced parameters.


    ![](/images/65930352/65930354.png)

     The following parameters are available:

    FASTQ URL(s)

    Semicolon-separated list of pathes to the input files.

    Output directory

    Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.

    Custom directory

    Select the custom output directory.

    List of adapters

    Specifies a non-default file which contains the list of adapter sequences which will be explicity searched against the library. The file must contain sets of named adapters in the form name\[tab\]sequence. Lines prefixed with a hash will be ignored.



    List of contaminants

    Specifies a non-default file which contains the list of contaminants to screen overrepresented sequences against. The file must contain sets of named contaminants in the form name\[tab\]sequence. Lines prefixed with a hash will be ignored.
