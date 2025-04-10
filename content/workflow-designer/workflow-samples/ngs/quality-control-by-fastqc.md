---
title: "Quality Control by FastQC"
weight: 600
---

# Quality Control by FastQC

FastQC aims to provide a simple way to perform quality control checks on raw sequence data from high throughput sequencing pipelines. It offers a set of analyses that you can use to quickly assess whether your data has any issues you should be aware of before conducting further analysis.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Quality Control by FastQC" can be found in the "NGS" section of the Workflow Designer samples.

##### Workflow Image

The workflow is as follows:

![](/images/65930352/65930353.png)

##### Workflow Wizard

The wizard has one page.

1. High Throughput Sequence QC Report by FastQC: On this page, you must input FASTQ file(s) and optionally modify advanced parameters.

   ![](/images/65930352/65930354.png)

   The following parameters are available:

   | Parameter           | Description                                                                                                                                   |
   |---------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
   | FASTQ URL(s)        | Semicolon-separated list of paths to the input files.                                                                                         |
   | Output directory    | Specify an output directory. Options include Custom (specify the output directory in the 'Custom directory' parameter), Workflow (internal workflow directory), or Input file (the directory of the input file). |
   | Custom directory    | Select the custom output directory.                                                                                                           |
   | List of adapters    | Specifies a non-default file containing the list of adapter sequences, which will be explicitly searched against the library. The file must contain sets of named adapters in the form name\[tab\]sequence. Lines prefixed with a hash will be ignored. |
   | List of contaminants| Specifies a non-default file containing the list of contaminants to screen overrepresented sequences against. The file must contain sets of named contaminants in the form name\[tab\]sequence. Lines prefixed with a hash will be ignored. |