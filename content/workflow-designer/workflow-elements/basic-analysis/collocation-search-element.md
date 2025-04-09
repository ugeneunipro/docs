---
title: "Collocation Search Element"
weight: 400
---

# Collocation Search Element

Finds groups of specified annotations in each supplied set of annotations, stores found regions as annotations.

**Element type:** collocated-annotation-search

## Parameters

| Parameter                | Description                                                                                              | Default value          | Parameter in Workflow File | Type      |
|--------------------------|----------------------------------------------------------------------------------------------------------|------------------------|----------------------------|-----------|
| **Result type**          | Copy original annotations or annotate found regions with new ones.                                       | Create new annotations | **result-type**            | _string_  |
| **Result annotation**    | Name of the result annotation to mark found collocations. **(Required)**                                 | misc_feature           | **result-name**            | _string_  |
| **Include boundaries**   | Include the most left and most right boundary annotations in the result or exclude them.                 | True                   | **include-boundary**       | _boolean_ |
| **Group of annotations** | List of annotation names to search. Found regions will contain all the named annotations. **(Required)** |                        | **annotations**            | _string_  |
| **Region size**          | Maximum allowed distance between the interesting annotations in a group.                                 | 1000                   | **region-size**            | _numeric_ |
| **Must fit into region** | Whether annotations must entirely fit within the specified region to form a group.                       | False                  | **must-fit**               | _boolean_ |

## Input/Output Ports

| Port Name (GUI)       | Workflow File Name | Slots                                                                                                      |
|-----------------------|--------------------|------------------------------------------------------------------------------------------------------------|
| **Input data**        | `in-sequence`      | **Sequence** → `sequence` (_sequence_)<br>**Set of annotations** → `annotations` (_annotation-table-list_) |
| **Group annotations** | `out-annotations`  | **Set of annotations** → `annotations` (_annotation-table_)                                                |
