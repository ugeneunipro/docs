---
title: "Search for TFBS"
weight: 300
---

# Search for TFBS

This sample demonstrates how to search for transcription factor binding sites (TFBS) using two different approaches - weight matrices and SITECON models - and to write the identified TFBS annotations into one output file.

The workflow involves the following steps:

1. The workflow reads the input sequences.
2. Each sequence is processed by the TFBS searching elements.
3. _Read Weight Matrix_ reads the input weight matrices, and _Read SITECON Model_ reads the input SITECON models. This data is also transferred to the TFBS searching elements.
4. Each TFBS searching element generates the corresponding annotations.
5. Subsequently, the two annotation data flows are multiplexed into one data flow.
6. The multiplexed data is written to the output file ("merged.gb" by default).

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Search for TFBS" can be found in the "Data Merging" section of the Workflow Designer samples.

##### Workflow Image

The workflow is illustrated as follows:

![](/images/65930296/65930297.png)

##### Workflow Wizard

The wizard comprises 3 pages.

1. **Input sequence(s):** On this page, you must input sequence(s).
   
   ![](/images/65930296/65930298.png)

2. **Search for TFBS parameters:** On this page, you can modify the parameters for searching TFBS.
   
   ![](/images/65930296/65930299.png)

   The following parameters are available:

   | Parameter             | Description                                                              |
   |-----------------------|--------------------------------------------------------------------------|
   | **Weight Matrix**     | Semicolon-separated list of paths to the input files.                    |
   | **Result annotation** | Annotation name for marking found regions.                               |
   | **Search in**         | Which strands should be searched: direct, complement, or both.           |
   | **Min score**         | Minimum score to detect a transcription factor binding site.             |
   | **SITECON model**     | Semicolon-separated list of paths to the input files.                    |
   | **Result annotation** | Annotation name for marking found regions.                               |
   | **Search in**         | Which strands should be searched: direct, complement, or both.           |
   | **Min score**         | Minimum score to detect a transcription factor binding site.             |
   | **Min err1**          | Alternative setting for filtering results: minimum value of Error type I.|
   |                       | Note that all thresholds (by score, err1, and err2) are applied when filtering results. |
   | **Max err2**          | Alternative setting for filtering results: maximum value of Error type II.|
   |                       | Note that all thresholds (by score, err1, and err2) are applied when filtering results. |

3. **Output data:** On this page, you can modify output parameters.
   
   ![](/images/65930296/65930300.png)

   The following parameters are available:

   | Parameter            | Description                                                                                       |
   |----------------------|---------------------------------------------------------------------------------------------------|
   | **Result file**      | Location of the output data file. If this attribute is set, the "Location" slot in the port will not be used. |
   | **Accumulate results** | Accumulate all incoming data in one file or create separate files for each input. In the latter case, an incremental numerical suffix is added to the file name. |
