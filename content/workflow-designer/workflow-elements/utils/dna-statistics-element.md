---
title: "DNA Statistics Element"
weight: 100
---

# DNA Statistics Element

Evaluates statistics for DNA sequences.

**Element type:** `dna-stats`

---

## Parameters

| **Parameter** | **Description**      | **Default Value** | **Parameter in Workflow File** | **Type**  |
|---------------|----------------------|-------------------|--------------------------------|-----------|
| GC-content    | Evaluate GC-content  | `True`            | `gc-content`                   | _boolean_ |
| GC1-content   | Evaluate GC1-content | `True`            | `gc1-content`                  | _boolean_ |
| GC2-content   | Evaluate GC2-content | `True`            | `gc2-content`                  | _boolean_ |
| GC3-content   | Evaluate GC3-content | `True`            | `gc3-content`                  | _boolean_ |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** _Input sequence_
- **Name in Workflow File:** `in-sequence`

| Slot In GUI | Slot in Workflow File | Type       |
|-------------|-----------------------|------------|
| Sequence    | `sequence`            | _sequence_ |

---

### Output Port

- **Name in GUI:** _Result annotation_
- **Name in Workflow File:** `out-annotations`

| Slot In GUI        | Slot in Workflow File | Type                    |
|--------------------|-----------------------|-------------------------|
| Set of annotations | `annotations`         | _annotation-table-list_ |
