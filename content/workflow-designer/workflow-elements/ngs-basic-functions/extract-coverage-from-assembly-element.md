---
title: "Extract Coverage from Assembly Element"
weight: 400
---

# Extract Coverage from Assembly Element

This workflow element extracts **coverage** and/or **base counts** from the incoming assembly data.

**Element type:** `extract-assembly-coverage`

---

## Parameters

| **Parameter**   | **Description**                                                                 | **Default Value**       | **Parameter in Workflow File** | **Type**  |
|-----------------|---------------------------------------------------------------------------------|-------------------------|--------------------------------|-----------|
| **Output file** | Path to the output data file. If this is set, slot `Location` will not be used. | `assembly_coverage.txt` | `url-out`                      | _string_  |
| **Export**      | Type of data to export: `coverage` or `base-count`.                             | `coverage`              | `export-type`                  | _string_  |
| **Threshold**   | Minimum coverage value to include in the output.                                | `1`                     | `threshold`                    | _numeric_ |

---

## Input/Output Ports

### Input Port

| **Name in GUI** | **Name in Workflow File** | **Slot**      | **Slot in Workflow File** | **Type**   |
|-----------------|---------------------------|---------------|---------------------------|------------|
| `in-assembly`   | `in-assembly`             | Assembly data | `assembly`                | _assembly_ |

### Output Port

_(None defined directly in the current schema – output is handled via the file path parameter `url-out`.)_

---

## Example

To extract base coverage from a single assembly file:

```bash
ugene workflow run \
  --element extract-assembly-coverage \
  --url-out ./coverage.txt \
  --export-type coverage \
  --threshold 5
```

This will output coverage data for all positions with at least 5x coverage.
