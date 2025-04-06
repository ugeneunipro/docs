---
title: "Weight Matrix"
weight: 1
---


# Weight Matrix

The _Weight Matrix_ plugin is a tool for solving the problem of a sequence annotating. As well as for the [_SITECON_](sitecon.md), the main use case of the plugin is recognition of potential transcription factor binding sites on basis of the data about conservative conformational and physicochemical properties revealed with the binding sites sets analysis.

The _Weight Matrix_ contains a lot of _position frequency matrices_ (PFM ‘s) and _position weight matrices_ (PWM ‘s, also known as _position specific score matrices_ — PSSM ‘s). The matrices came from two wide-known open archives: [JASPAR](http://jaspar.genereg.net/), which contains frequency matrices, and [UniPROBE](http://the_brain.bwh.harvard.edu/uniprobe/) containing weight matrices.

Also the _Weight Matrix_ plugin provides a tool for creating specific position frequency and weight matrices from an existing alignment or from a file with several sequences. The created matrix can be used as a profile for the search as well as the JASPAR and UNIPROBE ones.

To search for transcription factor binding sites in a DNA sequence select the _Analyze ‣ Search TFBS with matrices_ context menu item. The _Weight matrix search_ dialog will appear:


![](/images/65930906/65930907.png)

In the search dialog you must specify a file with PWM or PFM. You can do so by pressing the browse button and selecting the file.

Also you can use the [_special interface to choose a JASPAR matrix_](searching-jaspar-database.md) by pressing the _Search JASPAR database_ button.

Alternative way to specify the position weight/frequency matrix is to create a specific one from an alignment or a file with several sequences with the [_build a new matrix_](building-new-matrix.md) tool.

After the profile (the matrix) is loaded, you can adjust the threshold value. The threshold sets the minimal identity score for a result to pass. The more the result score is, the more it is homologically related to the aligned region. By changing the threshold you can filter low- scoring results.

If the loaded matrix is a position frequency matrix, you must also specify the algorithm to build the corresponding position weight matrix which will represent the transcription factor. There are four algorithms available.


![](/images/65930906/65930908.png)

Also you can add a selected matrix with the specified _Minimal score_ and the _Algorithm_ to the matrices list. To do it, select the matrix and other options and press the _Add to queue_ button. The plugin will search with all matrices specified in the list.

You can use the _Save list_ button to export the list of matrices to a \*.csv file. Later the list can be loaded from the file using the _Load list_ button.

The rest options are standard sequence search options: the strand and the sequence region where to search for matches.

After specifying the necessary options press the _Search_ button. The found results will appear in the dialog table. The corresponding results identity scores are in the _Score_ column.


![](/images/65930906/65930909.png)

Also you can see the matrix by using the _View matrix_ button:


![](/images/65930906/65930910.png)

The regions found by the weight matrix algorithm can be saved as annotations to the DNA sequence in the Genbank format by pressing the _Save as annotations_ button.

After saving, the file with resulting annotations will be automatically added to the current project, and the annotations will be added to the original sequence.

Note that in case of selecting JASPAR or UNIPROBE matrix, the resulting annotations will contain the given matrix properties.


![](/images/65930906/65930911.png)

See also:

*   [Searching JASPAR Database](searching-jaspar-database.md)
*   [Building New Matrix](building-new-matrix.md)



--------------------------------------------------------------------------------------------------------------------------------------------
