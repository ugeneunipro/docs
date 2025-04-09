---
title: "Export PHRED Qualities Element"
weight: 500
---

# Export PHRED Qualities Element

Export corresponding PHRED quality scores from input sequences.

**Element type:** export-phred-qualities

---

## Parameters

| **Parameter** | **Description**                         | **Default value** | **Parameter in Workflow File** | **Type** |
|---------------|-----------------------------------------|-------------------|--------------------------------|----------|
| PHRED output  | Path to file with PHRED quality scores. | –                 | url-out                        | _string_ |

---

## Input/Output Ports

### Input port

**Name in GUI:** DNA sequences
**Name in Workflow File:** in-sequence

| **Slot in GUI** | **Slot in Workflow File** | **Type** |
|-----------------|---------------------------|----------|
| Sequence        | sequence                  | _string_ |
