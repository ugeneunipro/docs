---
title: "LinkData Fetch"
weight: 400
---

# LinkData Fetch

This workflow fetches a sequence from LinkData using the specified work ID, filename, subject ID, and property ID, and writes the result into a file in FASTA format.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "LinkData Fetch" can be found in the "Custom Elements" section of the Workflow Designer samples.

##### Workflow Image

The workflow appears as follows:

![](/images/65930272/65930273.png)

##### Workflow Wizard

The wizard consists of 1 page.

1.  **LinkData Fetch:** On this page, you can modify the LinkData and output settings.

    ![](/images/65930272/65930274.png)

    The following parameters are available:

    | Parameter        | Description                                                                 |
    | ---------------- | --------------------------------------------------------------------------- |
    | Work ID          | Specifies the work ID.                                                      |
    | File Name        | Indicates the name of the file.                                             |
    | Subject          | Refers to the subject ID.                                                   |
    | Property         | Denotes the property ID.                                                    |
    | Result Sequence  | Location of the output data file. If this attribute is set, the "Location" slot in the port will not be used. |