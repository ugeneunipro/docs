---
title: "Find Repeated Elements"
weight: 1100
---

# Find Repeated Elements

This functionality identifies repetitions in each provided sequence and records the detected regions as annotations.

**Element Type:** `repeats-search`

---

## Parameters

| **Parameter**        | **Description**                                                                       | **Default Value** | **Parameter in Workflow File** | **Type**  |
|----------------------|---------------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| **Annotate as**      | Name of the result annotation for marking identified repeats.                         | `repeat_unit`     | `result-name`                  | _string_  |
| **Algorithm**        | Controls variations of the algorithm.                                                 | `Auto`            | `algorithm`                    | _numeric_ |
|                      | *0* - automatic selection<br>*1* - diagonal algorithm<br>*2* - suffix index algorithm |                   |                                |           |
| **Filter nested**    | Filters nested repeats.                                                               | `True`            | `filter-nested`                | _boolean_ |
| **Identity**         | Repeats identity percentage.                                                          | `100`             | `identity`                     | _numeric_ |
| **Inverted**         | Indicates whether to search for inverted repeats.                                     | `False`           | `inverted`                     | _boolean_ |
| **Max distance**     | Maximum distance between the repeats.                                                 | `5000`            | `max-distance`                 | _numeric_ |
| **Min distance**     | Minimum distance between the repeats.                                                 | `0`               | `min-distance`                 | _numeric_ |
| **Min length**       | Minimum length of the repeats.                                                        | `5`               | `min-length`                   | _numeric_ |
| **Parallel threads** | Number of parallel threads used for the task.                                         | `Auto (0)`        | `threads`                      | _numeric_ |
|                      | *0* = use the autodetected number of threads                                           |                   |                                |           |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `Input sequence`
- **Name in Workflow File:** `in-sequence`
- **Slots:**

  | Slot In GUI  | Slot in Workflow File | Type         |
  |--------------|------------------------|--------------|
  | Sequence     | `sequence`             | _sequence_   |

### Output Port

- **Name in GUI:** `Repeat annotations`
- **Name in Workflow File:** `out-annotations`
- **Slots:**

  | Slot In GUI         | Slot in Workflow File | Type                |
  |---------------------|------------------------|---------------------|
  | Set of annotations  | `annotations`          | _annotation-table_  |