---
title: "Extract Coverage from Assembly"
weight: 1
---


# Extract Coverage from Assembly

The workflow sample, described below, allows one to extract a coverage and/or bases count from an assembly. It receives a number of assemblies and for each of them produces coverage as a tab delimited plain text file. The coverage is extracted considering a threshold value.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Extract Coverage from Assembly" can be found in the "NGS" section of the Workflow Designer samples.

##### Workflow Image

The opened workflow looks as follows:


![](/images/65930345/65930346.png)

##### Workflow Wizard

The wizard has 3 pages.

1.  Input assembly (-ies) Page: On this page you must input assembly(-ies).


    ![](/images/65930345/65930347.png)

2.  Extract parameters Page: Here you can optionally modify extract parameters.


    ![](/images/65930345/65930348.png)

     The following parameters are available:

    Format

    Format to store the output.

    Export

    Data type to export.

    Threshold

    The minimum coverage value to export.

3.  Output data Page: On this page you can select an output file:


    ![](/images/65930345/65930349.png)
