---
title: "Find Correct Primer Pairs Element"
weight: 900
---

# Find Correct Primer Pairs Element

This element identifies correct primer pairs consisting of valid primers without dimers.

---

## Element Type

**Element type:** `find-primers`

---

## Parameters

| **Parameter**      | **Description**                | **Default Value** | **Parameter in Workflow File** | **Type** |
|--------------------|--------------------------------|-------------------|--------------------------------|----------|
| Output report file | Path to the report output file | *(none)*          | `output-file`                  | _string_ |

---

## Input/Output Ports

### Input Port

| **Name in GUI** | **Name in Workflow File** | **Slot** | **Slot in Workflow File** | **Type**   |
|-----------------|---------------------------|----------|---------------------------|------------|
| Input sequences | `in-sequence`             | Sequence | `sequence`                | _sequence_ |

---

This element can be used to ensure that primer design outputs only viable primer pairs suitable for PCR and other amplification workflows.