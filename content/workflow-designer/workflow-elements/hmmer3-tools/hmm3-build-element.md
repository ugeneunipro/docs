---
title: "HMM3 Build Element"
weight: 1
---


# HMM3 Build Element

Builds a HMM3 profile from a multiple sequence alignment. The HMM3 profile is a statistical model which captures position-specific information about how conserved each column of the alignment is, and which residues are likely.

**Element type:** hmm3-build

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Random seed**

Random generator seed. 0 - means that one-time arbitrary seed will be used.

0

**seed**

_numeric_

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

**Name in GUI:** _HMM3 profile_

**Name in Workflow File:** out-hmm3

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**HMM profile**

**hmm3-profile**

_hmm3-profile_
