---
title: "Group Primer Pairs Element"
weight: 1400
---

# Group Primer Pairs Element

Select groups of primer pairs that can be simultaneously used in one reaction tube.

The primers must be supplied in the following order: pair1_direct_primer, pair1_reverse_primer, pair2_direct_primer, pair2_reverse_primer, etc.

**Element type:** primers-grouper

| Parameter               | Description                        | Default value | Parameter in Workflow File | Type      |
|-------------------------|------------------------------------|---------------|----------------------------|-----------|
| **Output report file**  | Path to the report output file.    |               | **output-file**            | _string_  |

## Input/Output Ports

The element has 1 _input port_:

- **Name in GUI:** _Primer pairs_
- **Name in Workflow File:** in-sequence

**Slots:**

| Slot In GUI | Slot in Workflow File | Type       |
|-------------|-----------------------|------------|
| **Sequence** | **sequence**         | _sequence_ |