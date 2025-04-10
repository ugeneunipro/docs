---
title: "Align with Kalign Element"
weight: 400
---

# Align with Kalign Element

Aligns multiple sequence alignments (MSAs) using Kalign. Kalign is a fast and accurate multiple sequence alignment tool. The original version of the tool can be found at [http://msa.sbc.su.se](http://msa.sbc.su.se/).

**Element type:** kalign

## Parameters

| Parameter                 | Description                                                                                                                                  | Default value | Parameter in Workflow File | Type      |
|---------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Gap extension penalty** | The penalty for extending a gap.                                                                                                             | 8.52          | **gap-ext-penalty**        | _numeric_ |
| **Gap open penalty**      | The penalty for opening/closing a gap. Half the value will be subtracted from the alignment score when opening, and the other half when closing a gap. | 54.90         | **gap-open-penalty**       | _numeric_ |
| **Terminal gap penalty**  | The penalty to extend gaps from the N/C terminal of a protein or 5’/3’ terminal of nucleotide sequences.                                       | 4.42          | **terminal-gap-penalty**   | _numeric_ |
| **Bonus score**           | A bonus score that is added to each pair of aligned residues.                                                                                | 0.02          | **bonus-score**            | _numeric_ |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input MSA_  
**Name in Workflow File:** in-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |

And 1 _output port_:

**Name in GUI:** _Kalign result MSA_  
**Name in Workflow File:** out-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |