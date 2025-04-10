---
title: "Remote BLASTing"
weight: 1000
---

# Remote BLASTing

The workflow sample described below allows one to perform remote queries to the [NCBI BLAST database](http://blast.st-va.ncbi.nlm.nih.gov/Blast.cgi) to search for homologous nucleotide sequences for multiple input sequences simultaneously.

As a result of the BLAST, each input sequence is annotated with "blast result" annotations. These annotations are used to retrieve the corresponding homologous sequences from the NCBI database, based on the identifiers specified in the "blast result" annotations. The output homologous sequences and the original sequences, annotated by BLAST, are organized into folders.

### Environment Requirements

An internet connection is required to run this workflow sample.

### How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

#### Workflow Sample Location

The workflow sample "Remote BLASTing" can be found in the "Scenarios" section of the Workflow Designer samples.

#### Workflow Image

The opened workflow appears as follows:

![](/images/65930572/65930573.png)

#### Workflow Wizard

The wizard consists of 3 pages.

1. **Input Sequence(s) Page:** On this page, you must input at least one nucleotide sequence.

    ![](/images/65930572/65930574.png)

    **Example Input Data**

    For example, you can use the following two files as input for the workflow:
    * [my_sequence1.fa](/images/65930572/65930577.fa)
    * [my_sequence2.fa](/images/65930572/65930576.fa)

2. **Remote Nucleotide BLAST Page:** Here, you can optionally modify parameters for the remote BLAST queries. You can choose the search database, adjust the e-value, and set the maximum number of results (i.e., "Max hits"). The "Megablast" option, applied by default, optimizes the search for highly similar sequences only. Selecting it reduces search time, but some less similar results may be missed. Note that the "Megablast" option is also applied by default in the NCBI BLAST web interface.

    ![](/images/65930572/65930575.png)

    Additional parameters are available. A description of them can be found in the [Remote BLAST workflow element](../../workflow-elements/basic-analysis/remote-blast-element) chapter of the documentation.

    ![](/images/65930572/65930576.fa)

3. **Output Files Page:** This is an informational page. It indicates that this workflow has predefined names for the output files. For each input sequence, the workflow outputs:
    * **"orig_with_blast.gb" file:** This file contains the input sequence itself and the "blast result" annotations.
    * **"homologous.gb" file:** This file contains the homologous sequences retrieved from the [NCBI](http://www.ncbi.nlm.nih.gov/) by identifiers specified in the BLAST results.

   The results on the hard drive are organized into folders (see below).

   The wizard page looks as follows:

   ![](/images/65930572/65930577.fa)

#### Workflow Result

The workflow output files are displayed in the dashboard as follows:

![](/images/65930572/65930578.png)

Each file can be opened in the UGENE Sequence View by clicking on the corresponding link in the dashboard.

On the hard drive, the output is organized into folders named after the input sequences. For example, for the input sequences specified above, the output hierarchy will be as follows:

* _my_sequence1.fa_ folder with files:
  * _orig_with_blast.gb_
  * _homologous.gb_
* _my_sequence2.fa_ folder with files:
  * _orig_with_blast.gb_
  * _homologous.gb_