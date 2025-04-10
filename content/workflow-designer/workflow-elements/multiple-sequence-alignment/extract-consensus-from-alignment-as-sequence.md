---
title: "Extract Consensus from Alignment as Sequence"
weight: 800
---

# Extract Consensus from Alignment as Sequence

Extracts the consensus sequence from an incoming multiple sequence alignment (MSA) and outputs it as a sequence.

**Element type:** `extract-msa-consensus-sequence`

---

## Parameters

| **Parameter** | **Description**                                                   | **Default value** | **Parameter in Workflow File** | **Type**  |
|---------------|-------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| **Algorithm** | The algorithm used to calculate the consensus.                    | _(none)_          | `algorithm`                    | _string_  |
| **Threshold** | The threshold used by the algorithm (e.g., percentage agreement). | `100`             | `threshold`                    | _numeric_ |
| **Keep gaps** | Determines whether gaps should be kept in the resulting consensus sequence.  | `True`            | `keep-gaps`                    | _boolean_ |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `in-msa`
- **Name in Workflow File:** `in-msa`
- **Slots:**

| **Slot In GUI** | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|----------|
| MSA             | `msa`                     | _msa_    |

### Output Port

- **Name in GUI:** `out-sequence`
- **Name in Workflow File:** `out-sequence`
- **Slots:**

| **Slot In GUI** | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|----------|
| Sequence        | `sequence`                | _seq_    |