---
title: "Align with ClustalW Element"
weight: 1
---


# Align with ClustalW Element

Aligns multiple sequence alignments (MSAs) supplied with ClustalW.

ClustalW is a general-purpose multiple sequence alignment program for DNA or proteins. Visit [http://www.clustal.org/](http://www.clustal.org/) to learn more about it.

Clustal is used as an external tool from UGENE and it must be installed on your system. To learn more about the external tools, please, read the main [UGENE User Manual](http://ugene.unipro.ru/documentation.html).

**Element type:** clustalw

Parameters



Parameter

Description

Default value

Parameter in Workflow File

Type

**Weight matrix**

For proteins, it is a scoring table which describes the similarity of each amino acid to each other. For DNA it is the scores assigned to matches and mismatches.

default

**matrix**

_numeric_

Available values are:

*   0 - for IUB
*   1 - for ClustalW
*   2 - for BLOSUM
*   3 - for PAM
*   4 - for GONNET
*   5 - for ID
*   \-1 - for default matrix

**End gaps**

The penalty for closing a gap.

False

**close-gap-penalty**

_boolean_

**Gap distance**

The gap separation penalty. Tries to decrease the chances of gaps being too close to each other.

4.42

**gap-distance**

_numeric_

**Gap extension penalty**

The penalty for extending a gap.

8.52

**gap-ext-penalty**

_numeric_

**Gap open penalty**

The penalty for opening a gap.

53.90

**gap-open-penalty**

_numeric_

**Hydrophilic gaps off**

Hydrophilic gap penalties are used to increase the chances of a gap within a run (5 or more residues) of hydrophilic amino acids.

False

**no-hydrophilic-gaps**

_boolean_

**Residue-specific gaps off**

Residue-specific penalties are amino specific gap penalties that reduce or increase the gap opening penalties at each position in the alignment.

False

**no-residue-specific-gaps**

_boolean_

**Iteration type**

Alignment improvement iteration type.

None

**iteration-type**

_numeric_

Available values are:

*   0 - for None
*   1 - for Tree
*   2 - for Alignment

**Number of iterations**

The maximum number of iterations to perform.

3

**iterations-max-num**

_numeric_

**Tool path** (required)

Path to the ClustalW tool. The default path can be set in the UGENE Application Settings.

default

**path**

_string_

**Temporary directory**

Directory to store temporary files.

default

**temp-dir**

_string_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input MSA_

**Name in Workflow File:** in-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_

And 1 _output port_:

**Name in GUI:** _ClustalW result MSA_

**Name in Workflow File:** out-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_
