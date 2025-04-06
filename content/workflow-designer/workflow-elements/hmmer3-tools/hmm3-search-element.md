---
title: "HMM3 Search Element"
weight: 1
---


# HMM3 Search Element

Searches each input sequence for significantly similar sequence matches to all specified HMM profiles. In case several profiles were supplied, searches with all profiles one by one and output united set of annotations for each sequence.

**Element type:** hmm3-search

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Result annotation**

Name of the result annotations.

hmm\_signal

**result-name**

_string_

**Seed**

Random generator seed. 0 - means that one-time arbitrary seed will be used.

0

**seed**

_numeric_

**Filter by high E-value**

E-value filtering can be used to exclude low-probability hits from the result.

1e-1

**seqs-num**

_numeric_

**Filter by low score**

Score based filtering is an alternative to E-value filtering to exclude low-probability hits from the result.

0.01

**score**

_numeric_

Input/Output Ports

The element has 2 _input port_. The first gets the input sequence:

**Name in GUI:** _Input sequence_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

The second input port gets the HMM profile:

**Name in GUI:** _HMM3 profile_

**Name in Workflow File:** in-hmm3

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**HMM profile**

**hmm3-profile**

_hmm3-profile_

And 1 _output port_:

**Name in GUI:** _HMM3 annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
