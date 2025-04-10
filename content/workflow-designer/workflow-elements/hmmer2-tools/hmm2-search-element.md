---
title: "HMM2 Search Element"
weight: 200
---

# HMM2 Search Element

This element searches each input sequence for significantly similar sequence matches to all specified HMM profiles. If multiple profiles are provided, it searches with each profile individually and outputs a unified set of annotations for each sequence.

**Element type:** hmm2-search

## Parameters

| Parameter                      | Description                                                                                                      | Default Value      | Parameter in Workflow File | Type         |
|--------------------------------|------------------------------------------------------------------------------------------------------------------|--------------------|----------------------------|--------------|
| **Result annotation**          | Name of the result annotations.                                                                                   | hmm_signal         | **result-name**            | _string_     |
| **Filter by high E-value**     | E-value filtering can be used to exclude low-probability hits from the result.                                     | 1e-1               | **e-val**                  | _numeric_    |
| **Number of seqs**             | Calculates the E-value scores as if we had seen a sequence database of sequences.                                  | 1                  | **seqs-num**               | _numeric_    |
| **Filter by low score**        | Score-based filtering is an alternative to E-value filtering to exclude low-probability hits from the result.      | -1000000000.0      | **score**                  | _numeric_    |

## Input/Output Ports

The element has 2 _input ports_. 

The first port receives the input sequence:

- **Name in GUI:** _Input sequence_
- **Name in Workflow File:** in-sequence
- **Slots:**
  - Slot In GUI: **Sequence**
  - Slot in Workflow File: **sequence**
  - Type: _sequence_

The second input port receives the HMM profile:

- **Name in GUI:** _HMM profile_
- **Name in Workflow File:** in-hmm2
- **Slots:**
  - Slot In GUI: **HMM profile**
  - Slot in Workflow File: **hmm2-profile**
  - Type: _hmm2-profile_

And there is 1 _output port_:

- **Name in GUI:** _HMM annotations_
- **Name in Workflow File:** out-annotations
- **Slots:**
  - Slot In GUI: **Set of annotations**
  - Slot in Workflow File: **annotations**
  - Type: _annotation-table_