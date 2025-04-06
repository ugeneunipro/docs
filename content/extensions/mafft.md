---
title: "MAFFT"
weight: 1
---


# MAFFT

Originally, MAFFT is a multiple sequence alignment program for UNIX-like operating systems. However, currently, it is available for macOS, Linux, and Windows. It is used for both nucleotide and protein sequences.

**MAFFT homepage:** [http://mafft.cbrc.jp/alignment/software](http://mafft.cbrc.jp/alignment/software)

To make _MAFFT_ available from UGENE:

*   Install the _MAFFT_ program on your system.

*   Set the path to the _MAFFT_ executable on the [_External tools_](external-tools.md) tab of UGENE _[Application Settings](ugene-application-settings.md)_ dialog.

    For example, on Windows, you need to specify the path to the mafft.bat file.


To use _MAFFT_ open a multiple sequence alignment file and select the _Align with MAFFT_ item in the context menu or in the _Actions_ main menu. The following dialog appears:


![](/images/19759722/19894620.bmp)

The following parameters are available:

_Gap opening penalty_ — Gap opening penalty at group-to-group alignment.

_Offset (works like gap extension penalty)_ — offset value, which works like the gap extension penalty, for group-to-group alignment.

_Maximum number of iterative refine_ — specifies the number of cycles of iterative refinement to perform.
