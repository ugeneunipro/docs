---
title: "Align with ClustalO Element"
weight: 200
---


# Align with ClustalO Element

Aligns multiple sequence alignments (MSAs) supplied with ClustalO.

**Element type:** ClustalO

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Number of iterations**

Number of (combined guide-tree/HMM) iterations.

1

**num-iterations**

_numeric_

**Number of guidetree iterations**

Maximum number guidetree iterations.

0

**max-guidetree-iterations**

_numeric_

**Number of HMM iterations**

Maximum number of HMM iterations.

0

**max-hmm-iterations**

_numeric_

**Set auto options**

Set options automatically (might overwrite some of your options).

False

**set-auto**

_boolean_

**Tool path**

Path to the ClustalO tool.

The default path can be set in the UGENE application settings.

Default

**path**

_string_

**Temporary directory**

Directory to store temporary files.

Default

**temp-dir**

_string_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input MSA

**Name in Workflow File:** in-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_malignment_

And 1 _output port_:

**Name in GUI:** ClustalO result MSA

**Name in Workflow File:** out-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

__malignment__
