---
title: "Filter Element"
weight: 100
---

# Filter Element

This element passes through only data that matches the input filter value (or values).

**Element type:** `filter-by-values`

---

## Parameters

| **Parameter**      | **Description**                                     | **Default Value** | **Parameter in Workflow File** | **Type** |
|--------------------|-----------------------------------------------------|-------------------|--------------------------------|----------|
| Filter by value(s) | Semicolon-separated list of values used for filter. | *(none)*          | `text`                         | _string_ |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `Input values`
- **Name in Workflow File:** `in-data`

| Slot In GUI  | Slot in Workflow File | Type     |
|--------------|-----------------------|----------|
| Input values | `text`                | _string_ |

### Output Port

- **Name in GUI:** `Passing values (by Filter)`
- **Name in Workflow File:** `filtered-data`

| Slot In GUI       | Slot in Workflow File        | Type                                  |
|-------------------|------------------------------|---------------------------------------|
| *(same as input)* | *(not explicitly specified)* | *(inferred from context as _string_)* |
