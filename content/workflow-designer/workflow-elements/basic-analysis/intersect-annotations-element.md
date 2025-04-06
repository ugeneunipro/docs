---
title: "Intersect Annotations Element"
weight: 1
---


# Intersect Annotations Element

Intersects two sets of annotations denoted as A and B.

**Element type:** intersect-annotations

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Result annotations**

Select one of the following:

*   Shared interval to report intervals shared between overlapped annotations from set A and set B.
*   Overlapped annotations from A to report annotations from set A that have an overlap with annotations from set B.
*   Non-overlapped annotations from A to report annotations from set A that have NO overlap with annotations from set B.

Overlapped annotations from set A

**report**

_numeric_

**Unique overlaps**

If the parameter value is "True", write original A entry once if any overlaps found in B. In other words, just report the fact at least one overlap was found in B.
The minimum overlap number is ignored in this case.

If the parameter value is "False", the A annotation is reported for every overlap found.

True

**unique**

_boolean_

**Minimum overlap**

Minimum overlap required as a fraction of an annotation from set A.
By default, even 1 bp overlap between annotations from set A and set B is taken into account. Yet sometimes you may want to restrict reported overlaps to cases where the annotations in B overlaps at least X% (e.g. 50%) of the A annotation. This parameter is only available if the parameter "Unique overlaps" is "False".

0.0000001%

**minimum-overlap**

_numeric_

Input/Output Ports
------------------

**Name in GUI:** Annotations AThe element has 2 _input ports_:

**Name in Workflow File:** input-annotations-a

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Annotations A**

**annotations**

_annotation-table_

**Name in GUI:** Annotations B

**Name in Workflow File:** input-annotations-b

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Annotations B**

**annotations**

_annotation-table_

And 1 _output port_:

**Name in GUI:** Annotations

**Name in Workflow File:** output-intersect-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Annotations**

**annotations**

_annotation-table_
