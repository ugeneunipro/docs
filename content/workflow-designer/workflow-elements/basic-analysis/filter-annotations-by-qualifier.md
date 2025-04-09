---
title: "Filter Annotations by Qualifier"
weight: 800
---

# Filter Annotations by Qualifier

Filters annotations by qualifier.

**Element type:** `filter-annotations-by-qualifier`

---

## Parameters

| **Parameter**    | **Description**                                                                 | **Default Value** | **Parameter in Workflow File** | **Type**  |
|------------------|---------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| Qualifier name   | Name of the qualifier to use for filtering.                                     | *(none)*          | `qualifier-name`               | _string_  |
| Qualifier value  | Text value of the qualifier to apply as filtering criteria.                     | *(none)*          | `qualifier-value`              | _string_  |
| Accept or filter | Selects the name filter: accept specified names or accept all except specified. | `True`            | `accept-or-filter`             | _boolean_ |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `Input annotations`
- **Name in Workflow File:** `in-annotations`

| Slot In GUI        | Slot in Workflow File | Type               |
|--------------------|-----------------------|--------------------|
| Set of annotations | `annotations`         | _annotation-table_ |

### Output Port

- **Name in GUI:** `Result annotations`
- **Name in Workflow File:** `out-annotations`

| Slot In GUI        | Slot in Workflow File | Type               |
|--------------------|-----------------------|--------------------|
| Set of annotations | `annotations`         | _annotation-table_ |
