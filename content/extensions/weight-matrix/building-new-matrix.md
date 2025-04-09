---
title: "Building New Matrix"
weight: 200
---


# Building New Matrix

To create a position weight or frequency matrix from an alignment or a file with several sequences, press the _Build new matrix_ button in the _Weight matrix search_ dialog, or select the _Tools ‣ Search for TFBS ‣ Build weight matrix_ main menu item:


![](/images/65930915/65930916.png)

The _Build weight or frequency matrix_ dialog will appear:


![](/images/65930915/65930917.png)

The following parameters are available:

_Input file_ — an alignment or a file with several sequences to build the matrix from. The parameter is mandatory.

_Output file_ — the resulting matrix will be saved in this file. The parameter is mandatory.

_Statistic type_ — defines the way in which the statistics will be collected. The _Mononucleic_ option is basically good for small alignments, and the _Dinucleic_ option must give more appropriate results for big alignments.

_Matrix type_ — defines the type of the resulting matrix.

If the _Frequency matrix_ option is selected then the frequency matrix will be created and saved into the resulting file.

If the _Weight matrix_ option is selected then the intermediate frequency matrix will be created and then transformed into a weight matrix on basis of the selected _Weight algorithm_. Then the weight matrix will be saved into the resulting file.

For some input files the colored “Alignment Logo” appears at the bottom of the dialog. It gives the representation of the selected alignment.


![](/images/65930915/65930918.png)

The “Alignment logo” appears when:

*   The input file format is \*.pfm, \*.aln or it is a file with several sequences;
*   The size of the input file is small enough.

To start the operation, press the _Start_ button. The matrix will be created and saved. If the _Build weight or frequency matrix_ dialog was invoked from the _Weight matrix search_ dialog, then the matrix also will be chosen as the current profile.
