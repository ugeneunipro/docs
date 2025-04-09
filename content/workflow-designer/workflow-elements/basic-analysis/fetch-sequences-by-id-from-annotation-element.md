---
title: "Fetch Sequences by ID From Annotation Element"
weight: 600
---

# Fetch Sequences by ID From Annotation Element

Parses annotations to find any IDs and fetches corresponding sequences.

**Element type:** `fetch-sequence`

---

## Parameters

| **Parameter**          | **Description**                                              | **Default Value** | **Parameter in Workflow File** | **Type** |
|------------------------|--------------------------------------------------------------|-------------------|--------------------------------|----------|
| Save file to directory | The directory to store sequence files loaded from a database | `default`         | `save-dir`                     | _string_ |
| NCBI database          | The database to read from                                    | `nucleotide`      | `database`                     | _string_ |

Available values for **NCBI database**:

- `nucleotide`
- `protein`

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `Input annotations`
- **Name in Workflow File:** `in-annotations`

| Slot In GUI        | Slot in Workflow File | Type               |
|--------------------|-----------------------|--------------------|
| Set of annotations | `annotations`         | _annotation-table_ |

### Output Port

- **Name in GUI:** `Sequence`
- **Name in Workflow File:** `out-sequence`

| Slot In GUI        | Slot in Workflow File | Type               |
|--------------------|-----------------------|--------------------|
| Set of annotations | `annotations`         | _annotation-table_ |
| Sequence           | `sequence`            | _sequence_         |
