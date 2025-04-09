---
title: "File Format Conversion Element"
weight: 300
---

# File Format Conversion Element

Converts the file to the selected format if it is not excluded.

**Element type:** `files-conversion`

---

## Parameters

| **Parameter**    | **Description**                                                   | **Default Value** | **Parameter in Workflow File** | **Type** |
|------------------|-------------------------------------------------------------------|-------------------|--------------------------------|----------|
| Document format  | Document format of the output file.                               | *(none)*          | `document-format`              | _string_ |
| Excluded formats | The input file won't be converted to any of the selected formats. | *(none)*          | `excluded-formats`             | _string_ |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `File`
- **Name in Workflow File:** `in-file`

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| Source URL  | `input-url`           | _string_ |

### Output Port

- **Name in GUI:** `File`
- **Name in Workflow File:** `out-file`

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| Source URL  | `output-url`          | _string_ |
