---
title: "HMM3 Search Element"
weight: 200
---

# HMM3 Search Element

This element searches each input sequence for significantly similar matches to all specified HMM profiles. If several profiles are provided, the element searches with each profile one by one and outputs a unified set of annotations for each sequence.

**Element type:** hmm3-search

## Parameters

| Parameter                | Description                                                                                            | Default value | Parameter in Workflow File | Type          |
|--------------------------|--------------------------------------------------------------------------------------------------------|---------------|---------------------------|---------------|
| **Result annotation**    | Name for the result annotations.                                                                       | hmm_signal    | **result-name**            | _string_      |
| **Seed**                 | Random generator seed. A value of 0 indicates that a one-time arbitrary seed will be used.            | 0             | **seed**                   | _numeric_     |
| **Filter by high E-value** | E-value filtering can be used to exclude low-probability hits from the results.                      | 1e-1          | **seqs-num**               | _numeric_     |
| **Filter by low score**  | Score-based filtering serves as an alternative to E-value filtering to exclude low-probability hits.  | 0.01          | **score**                  | _numeric_     |

## Input/Output Ports

The element has two _input ports_. The first port receives the input sequence:

- **Name in GUI:** _Input sequence_
- **Name in Workflow File:** in-sequence

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| **Sequence**| **sequence**          | _sequence_|

The second input port receives the HMM profile:

- **Name in GUI:** _HMM3 profile_
- **Name in Workflow File:** in-hmm3

| Slot In GUI     | Slot in Workflow File | Type           |
|-----------------|-----------------------|----------------|
| **HMM profile** | **hmm3-profile**      | _hmm3-profile_ |

The element also has one _output port_:

- **Name in GUI:** _HMM3 annotations_
- **Name in Workflow File:** out-annotations

| Slot In GUI         | Slot in Workflow File | Type             |
|---------------------|-----------------------|------------------|
| **Set of annotations** | **annotations**    | _annotation-table_ |