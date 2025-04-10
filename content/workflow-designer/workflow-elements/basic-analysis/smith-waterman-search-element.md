---
title: "Smith-Waterman Search Element"
weight: 2200
---

# Smith-Waterman Search Element

This element searches for regions in a sequence that are similar to a pattern sequence and outputs a set of annotations. It uses the well-known Smith-Waterman algorithm for performing local sequence alignment.

**Element type:** ssearch

## Parameters

| Parameter                         | Description                                                                                   | Default value               | Parameter in Workflow File | Type    |
|-----------------------------------|-----------------------------------------------------------------------------------------------|-----------------------------|----------------------------|---------|
| **Substitution Matrix**           | Describes the rate at which one character in a sequence changes to other character states over time. | Auto                        | **matrix**                 | _string_|
|                                   | Available values are:                                                                        |                             |                            |         |
|                                   | - Auto - for auto detecting matrix                                                           |                             |                            |         |
|                                   | - blosum60                                                                                   |                             |                            |         |
|                                   | - dna                                                                                        |                             |                            |         |
|                                   | - rna                                                                                        |                             |                            |         |
| **Algorithm**                     | Version of the Smith-Waterman algorithm. Use optimized versions (SSE, Classic2) if supported. | SSE2                        | **algorithm**              | _string_|
|                                   | Available values are:                                                                        |                             |                            |         |
|                                   | - Classic 2                                                                                  |                             |                            |         |
|                                   | - SSE2                                                                                       |                             |                            |         |
| **Filter Results**                | Specifies whether to filter the intersected results or to return all the results.             | filter-intersections        | **filter-strategy**        | _string_|
|                                   | Available values are:                                                                        |                             |                            |         |
|                                   | - filter-intersections                                                                      |                             |                            |         |
|                                   | - none                                                                                       |                             |                            |         |
| **Min Score**                     | Minimal percent similarity between a sequence and a pattern.                                  | 90%                         | **min-score**              | _numeric_|
| **Search in**                     | Specifies which strands should be searched: direct, complementary, or both.                   | both strands                | **strand**                 | _numeric_|
|                                   | Available values are:                                                                        |                             |                            |         |
|                                   | - 0 - for searching in both strands                                                          |                             |                            |         |
|                                   | - 1 - for searching in the direct strand                                                     |                             |                            |         |
|                                   | - 2 - for searching in the complement strand                                                 |                             |                            |         |
| **Search in Translation**         | Translates a supplied nucleotide sequence to protein and searches in the translated sequence. | False                       | **amino**                  | _boolean_|
| **Gap Open Score**                | Penalty for opening a gap.                                                                    | -10.0                       | **gap-open-score**         | _numeric_|
| **Gap Extension Score**           | Penalty for extending a gap.                                                                  | -1.0                        | **gap-ext-score**          | _numeric_|
| **Use Pattern Names**             | Use a pattern name as an annotation name.                                                     | True                        | **use-names**              | _boolean_|
| **Annotate as**                   | Name of the result annotations.                                                               | misc_feature                | **result-name**            | _string_|
| **Qualifier name for pattern name** | Name of the qualifier in result annotations that contains a pattern name.                    | pattern name                | **pattern-name-qual**      | _string_|

## Input/Output Ports

The element has 2 _input ports._ The first input port:

**Name in GUI:** _Input data_

**Name in Workflow File:** in-sequence

**Slots:**

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|------------------------|----------|
| **Sequence**| **sequence**           | _sequence_|

The second input port:

**Name in GUI:** _Pattern data_

**Name in Workflow File:** pattern

**Slots:**

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|------------------------|----------|
| **Sequence**| **sequence**           | _sequence_|

And 1 _output port_:

**Name in GUI:** _Pattern annotations_

**Name in Workflow File:** out-annotations

**Slots:**

| Slot In GUI        | Slot in Workflow File | Type             |
|--------------------|------------------------|------------------|
| **Set of annotations** | **annotations**     | _annotation-table_ |