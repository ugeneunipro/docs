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

- **Input file** — an alignment or a file with several sequences to build the matrix from. This parameter is mandatory.
- **Output file** — the resulting matrix will be saved in this file. This parameter is mandatory.
- **Statistic type** — defines how the statistics will be collected. The _Mononucleic_ option is generally good for small alignments, while the _Dinucleic_ option should give more appropriate results for large alignments.
- **Matrix type** — defines the type of the resulting matrix.

  - If the _Frequency matrix_ option is selected, then the frequency matrix will be created and saved in the resulting file.
  - If the _Weight matrix_ option is selected, then an intermediate frequency matrix will be created and then transformed into a weight matrix based on the selected _Weight algorithm_. The weight matrix will then be saved into the resulting file.

For some input files, the colored “Alignment Logo” appears at the bottom of the dialog. It provides a representation of the selected alignment.

![](/images/65930915/65930918.png)

The “Alignment Logo” appears when:

- The input file format is \*.pfm, \*.aln, or it is a file with several sequences.
- The size of the input file is small enough.

To start the operation, press the _Start_ button. The matrix will be created and saved. If the _Build weight or frequency matrix_ dialog was invoked from the _Weight matrix search_ dialog, then the matrix will also be chosen as the current profile.