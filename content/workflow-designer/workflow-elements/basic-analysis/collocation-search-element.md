---
title: "Collocation Search Element"
weight: 400
---

# Collocation Search Element

The Collocation Search Element finds groups of specified annotations within each supplied set of annotations and stores the identified regions as annotations.

**Element type:** collocated-annotation-search

## Parameters

| Parameter                | Description                                                                                              | Default Value          | Parameter in Workflow File | Type      |
|--------------------------|----------------------------------------------------------------------------------------------------------|------------------------|----------------------------|-----------|
| **Result type**          | Choose to copy the original annotations or to annotate the found regions with new ones.                  | Create new annotations | **result-type**            | _string_  |
| **Result annotation**    | Name of the result annotation to mark found collocations. **(Required)**                                 | misc_feature           | **result-name**            | _string_  |
| **Include boundaries**   | Include the leftmost and rightmost boundary annotations in the result or exclude them.                   | True                   | **include-boundary**       | _boolean_ |
| **Group of annotations** | List of annotation names to search. Found regions will contain all the named annotations. **(Required)** |                        | **annotations**            | _string_  |
| **Region size**          | Maximum allowed distance between the interesting annotations in a group.                                 | 1000                   | **region-size**            | _numeric_ |
| **Must fit into region** | Whether annotations must entirely fit within the specified region to form a group.                       | False                  | **must-fit**               | _boolean_ |

## Input/Output Ports

| Port Name (GUI)       | Workflow File Name | Slots                                                                                                      |
|-----------------------|--------------------|------------------------------------------------------------------------------------------------------------|
| **Input data**        | `in-sequence`      | **Sequence** → `sequence` (_sequence_)<br>**Set of annotations** → `annotations` (_annotation-table-list_) |
| **Group annotations** | `out-annotations`  | **Set of annotations** → `annotations` (_annotation-table_)                                                |