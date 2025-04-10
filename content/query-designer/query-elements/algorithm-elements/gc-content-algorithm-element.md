---
title: "GC Content Algorithm Element"
weight: 300
---

# GC Content Algorithm Element

Identifies regions in a sequence where the GC content falls within a specified range.

---

## Parameters in GUI

| **Parameter**      | **Description**                                  | **Default Value** |
|--------------------|--------------------------------------------------|-------------------|
| **Min GC content** | Minimum GC content value in percentage.          | 20%               |
| **Max GC content** | Maximum GC content value in percentage.          | 40%               |
| **Min length**     | Minimum length of a region in base pairs.        | 50 bp             |
| **Max length**     | Maximum length of a region in base pairs.        | 1000 bp           |

---

## Parameters in Schema File

**Element type:** `find-gc`

| **Parameter in Schema File** | **Parameter in GUI** | **Type**  |
|------------------------------|----------------------|-----------|
| `region-start`               | Min GC content       | _numeric_ |
| `region-end`                 | Max GC content       | _numeric_ |
| `min-len`                    | Min length           | _numeric_ |
| `max-len`                    | Max length           | _numeric_ |