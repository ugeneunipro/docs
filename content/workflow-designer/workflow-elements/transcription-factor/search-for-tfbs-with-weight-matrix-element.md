---
title: "Search for TFBS with Weight Matrix Element"
weight: 900
---

# Search for TFBS with Weight Matrix Element

This feature searches each input sequence for transcription factor binding sites that are significantly similar to specified weight matrices. If multiple profiles are provided, the feature searches with all profiles one by one and outputs a merged set of annotations for each sequence.

**Element type:** wmatrix-search

Parameters
----------

| Parameter       | Description                                                                                  | Default value     | Parameter in Workflow File | Type   |
|-----------------|----------------------------------------------------------------------------------------------|-------------------|----------------------------|--------|
| **Result annotation** | Name of the result annotations.                                                         | misc\_feature     | **result-name**            | _string_ |
| **Search in**   | Specifies which strands should be searched: direct, complement, or both.                     | both strands      | **strand**                 | _numeric_ |
| **Min score**   | Minimum score to detect transcription factor binding site as a percentage.                   | 85                | **min-score**              | _numeric_ |

Available values for "Search in" are:

- 0 - for searching in both strands
- 1 - for searching in the direct strand
- 2 - for searching in the complement strand

Input/Output Ports

The element has 2 _input ports_. The first port:

**Name in GUI:** _Sequence_

**Name in Workflow File:** in-sequence

**Slots:**

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| **Sequence** | **sequence**          | _sequence_ |

The second input port receives the SITECON model:

**Name in GUI:** _Weight matrix_

**Name in Workflow File:** in-wmatrix

**Slots:**

| Slot In GUI    | Slot in Workflow File | Type     |
|----------------|-----------------------|----------|
| **Weight matrix** | **wmatrix**         | _wmatrix_ |

And there is 1 _output port_:

**Name in GUI:** _Weight matrix annotations_

**Name in Workflow File:** out-annotations

**Slots:**

| Slot In GUI         | Slot in Workflow File | Type               |
|---------------------|-----------------------|--------------------|
| **Set of annotations** | **annotations**      | _annotation-table_ |