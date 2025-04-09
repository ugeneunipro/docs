---
title: "HMM2 Search Element"
weight: 200
---


# HMM2 Search Element

Searches each input sequence for significantly similar sequence matches to all specified HMM profiles. In case several profiles were supplied, searches with all profiles one by one and output united set of annotations for each sequence

**Element type:** hmm2-search

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

**Filter by high E-value**

E-value filtering can be used to exclude low-probability hits from result.

1e-1

**e-val**

_numeric_

**Number of seqs**

Calculates the E-value scores as if we had seen a sequence database of sequences.

1

**seqs-num**

_numeric_

**Filter by low score**

Score based filtering is an alternative to E-value filtering to exclude low-probability hits from result.

\-1000000000.0

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

**Name in GUI:** _HMM profile_

**Name in Workflow File:** in-hmm2

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**HMM profile**

**hmm2-profile**

_hmm2-profile_

And 1 _output port_:

**Name in GUI:** _HMM annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
