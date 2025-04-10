---
title: "Extract Consensus from Alignment as Text"
weight: 900
---

# Extract Consensus from Alignment as Text

Extract the consensus string from an incoming multiple sequence alignment (MSA) and output it as plain text.

**Element type:** `extract-msa-consensus-string`

---

## Parameters

| **Parameter** | **Description**                                                   | **Default value** | **Parameter in Workflow File** | **Type**  |
|---------------|-------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| **Algorithm** | The algorithm used to calculate the consensus.                    | _(none)_          | `algorithm`                    | _string_  |
| **Threshold** | The threshold used by the algorithm (e.g., percentage agreement). | `100`             | `threshold`                    | _numeric_ |

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
- **Name in Workflow File:** `out-text`
- **Slots:**

| **Slot In GUI** | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|----------|
| Plain text      | `text`                    | _string_ |