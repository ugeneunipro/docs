---
title: "ClustalO"
weight: 1
---


# ClustalO

Clustal is a widely used multiple sequence alignment program. It is used for both nucleotide and protein sequences.Clustal Omega is the latest addition to the Clustal family. It offers a significant increase in scalability over previous versions, allowing hundreds of thousands of sequences to be aligned in only a few hours. It will also make use of multiple processors, where present.

**Clustal home page:** [http://www.clustal.org](http://www.clustal.org/)

If you are using Windows OS, there are no additional configuration steps required, as _ClustalO_ executable file is included to the UGENE distribution package. Otherwise:

*   Install the _Clustal_ program on your system.
*   Set the path to the _ClustalW_ executable on the [_External tools_](external-tools-plugin.md) tab of UGENE [_Application Settings_](ugene-application-settings.md) dialog.

Now you are able to use _ClustaOl_ from UGENE.

Open a multiple sequence alignment file and select the _Align with ClustalO_ item in the context menu or in the _Actions_ main menu. The _Align with ClustalO_ dialog will appear (see below), where you can adjust the following parameters:

_Number of iterations_ — number of (combined guide tree/HMM) iterations.

_Max number guidetree iterations_ — maximum guide tree iterations.

_Max number of HMM iterations_ —maximum number of HMM iterations.

_Number of CPUs being used -_ number of processors to use.

_Set options automatically -_ set options automatically (might overwrite some of your options).


![](/images/6062194/6258701.png)
