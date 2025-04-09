---
title: "Align with T-Coffee Element"
weight: 700
---


# Align with T-Coffee Element

T-Coffee is a multiple sequence alignment package.

T-Coffee is used as an external tool from UGENE and it must be installed on your system. To learn more about the external tools, please, read main [UGENE User Manual](http://ugene.unipro.ru/documentation.html).

**Element type:** tcoffee

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Gap extension penalty**

Gap Extension Penalty. Positive values give rewards to gaps and prevent the alignment of unrelated segments.

0

**gap-ext-penalty**

_numeric_

**Gap open penalty**

Gap open penalty. Must be negative, best matches get a score of 1000.

\-50

**gap-open-penalty**

_numeric_

**Max iteration**

Number of iteration on the progressive alignment. 0 - no iteration, -1 - Nseq iterations.

0

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

**Name in GUI:** _Multiple sequence alignment_

**Name in Workflow File:** out-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_
