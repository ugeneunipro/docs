---
title: "Dump Sequence Info"
weight: 300
---


# Dump Sequence Info

This workflow dump sequence name and sequence size to output for all incoming sequences.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Dump Sequence Info" can be found in the "Custom Elements" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930268/65930269.png)

##### Workflow Wizard

The wizard has 2 pages.

1.  Input sequence(s): On this page you must input sequence(s).


    ![](/images/65930268/65930270.png)

2.  Output data: On this page you can modify output settings.


    ![](/images/65930268/65930271.png)

    The following parameters are available:

    Result file

    Location of output data file. If this attribute is set, slot "Location" in port will not be used.

    Accumulate results

    Accumulate all incoming data in one file or create separate files for each input.In the latter case, an incremental numerical suffix is added to the file name.
