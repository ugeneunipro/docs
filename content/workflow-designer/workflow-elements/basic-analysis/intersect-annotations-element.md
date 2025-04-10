---
title: "Intersect Annotations Element"
weight: 1600
---

# Intersect Annotations Element

Intersects two sets of annotations denoted as A and B.

**Element type:** intersect-annotations

Parameters
----------

| Parameter              | Description                                                                                                                                                                                                                                                                                                                                                                | Default value                       | Parameter in Workflow File |
|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------|----------------------------|
| **Result annotations** | Select one of the following: <ul><li>Shared interval to report intervals shared between overlapped annotations from set A and set B.</li><li>Overlapped annotations from A to report annotations from set A that have an overlap with annotations from set B.</li><li>Non-overlapped annotations from A to report annotations from set A that have NO overlap with annotations from set B.</li></ul> | Overlapped annotations from set A   | **report**                 | _numeric_                  |
| **Unique overlaps**    | If the parameter value is "True," write the original A entry once if any overlaps are found in B. In other words, just report the fact that at least one overlap was found in B. The minimum overlap number is ignored in this case. If the parameter value is "False," the A annotation is reported for every overlap found.                                                            | True                               | **unique**                 | _boolean_                  |
| **Minimum overlap**    | Minimum overlap required as a fraction of an annotation from set A. By default, even 1 bp overlap between annotations from set A and set B is taken into account. Yet, sometimes you may want to restrict reported overlaps to cases where the annotations in B overlap at least X% (e.g., 50%) of the A annotation. This parameter is only available if the parameter "Unique overlaps" is "False."       | 0.0000001%                         | **minimum-overlap**        | _numeric_                  |

Input/Output Ports
------------------

The element has 2 _input ports_:

| Name in GUI      | Name in Workflow File   | Slots         | Slot In GUI | Slot in Workflow File | Type             |
|------------------|-------------------------|---------------|-------------|-----------------------|------------------|
| Annotations A    | input-annotations-a     | **annotations** | Annotations A | annotations           | _annotation-table_ |
| Annotations B    | input-annotations-b     | **annotations** | Annotations B | annotations           | _annotation-table_ |

And 1 _output port_:

| Name in GUI    | Name in Workflow File          | Slots         | Slot In GUI | Slot in Workflow File | Type             |
|----------------|--------------------------------|---------------|-------------|-----------------------|------------------|
| Annotations    | output-intersect-annotations  | **annotations** | Annotations | annotations           | _annotation-table_ |