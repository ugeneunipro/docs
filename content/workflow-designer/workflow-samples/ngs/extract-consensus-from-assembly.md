---
title: "Extract Consensus from Assembly"
weight: 1
---


# Extract Consensus from Assembly

The workflow sample, described below, uses input assemblies to extract the consensus and save them to a FASTA.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Extract Consensus from Assembly" can be found in the "NGS" section of the Workflow Designer samples.

##### Workflow Image

The opened workflow looks as follows:


![](/images/65930342/65930343.png)

##### Workflow Wizard

The wizard has 1 page.

1.  Extract Consensus Page: On this page you must input assembly file and output file. Also you can modify other input parameters.


    ![](/images/65930342/65930344.png)

     The following parameters are available:

    Assembly

    Semicolon-separated list of pathes to the input files.

    Algorithm

    The algorithm of consensus extracting.

    Keep gaps

    Set this parameter if the result consensus must keep the gaps.

    Output files

    Location of output data file. If this attribute is set, slot "Location" in port will not be used.
