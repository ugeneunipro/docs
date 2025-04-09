---
title: "Convert UQL Schema Results to Alignment"
weight: 300
---


# Convert UQL Schema Results to Alignment

This schema allows to analyze sequence with Query and save results as alignment of selected features.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Convert UQL Schema Results to Alignment" can be found in the "Conversions" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930255/65930256.png)

##### Workflow Wizard

The wizard has 2 pages.

1.  Input sequence(s): On this page you must input sequence(s).


    ![](/images/65930255/65930257.png)

2.  Annotate with UQL: On this page you can modify annotation and output settings.


    ![](/images/65930255/65930258.png)

    The following parameters are available:

    UQL schema file

    Schema file.

    Merge

    Merges regions of each result into single annotation if true.

    Offset

    Specifies left and right offsets for merged annotation (if 'Merge' parameter is set to true).

    Annotation names

    File with annotation names, separated with whitespaces or list of annotation names which will be accepted or filtered. Use space as the separator.

    Accept or filter

    Selects the name filter: accept specified names or accept all except specified.

    Result file

    Location of output data file. If this attribute is set, slot "Location" in port will not be used.

    Document format

    Document format of output file.
