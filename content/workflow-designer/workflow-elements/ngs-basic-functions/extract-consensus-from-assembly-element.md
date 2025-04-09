---
title: "Extract Consensus from Assembly Element"
weight: 300
---

# Extract Consensus from Assembly Element

Extracts the consensus sequence from the incoming assembly.

---

## Element Type

**Element type:** `extract-consensus`

---

## Parameters

| **Parameter** | **Description**                                           | **Default Value** | **Parameter in Workflow File** | **Type**  |
|---------------|-----------------------------------------------------------|-------------------|--------------------------------|-----------|
| **Algorithm** | The algorithm of consensus extracting.                    | Default           | `algorithm`                    | _string_  |
| **Keep gaps** | If set to `True`, the result consensus will contain gaps. | True              | `keep-gaps`                    | _boolean_ |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `in-assembly`
- **Name in Workflow File:** `in-assembly`

| **Slot In GUI** | **Slot in Workflow File** | **Type**   |
|-----------------|---------------------------|------------|
| Assembly data   | `assembly`                | _assembly_ |

---

### Output Port

- **Name in GUI:** `out-sequence`
- **Name in Workflow File:** `out-sequence`

| **Slot In GUI** | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|----------|
| Sequence        | `sequence`                | _string_ |
