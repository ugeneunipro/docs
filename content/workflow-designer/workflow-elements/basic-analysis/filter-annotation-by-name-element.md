---
title: "Filter Annotation by Name Element"
weight: 700
---


# Filter Annotation by Name Element

Filters annotations by name.

**Element type:** filter-annotations

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Annotation names**

List of annotation names, separated by spaces, that will be accepted or filtered.



**annotation-names**

_string_

**Annotation names file**

File with annotation names, separated with whitespaces which will be accepted or filtered.



**annotation-names-file**

_string_

**Accept or filter**

Selects the name filter: accept specified names or accept all except specified.

True

**accept-or-filter**

_boolean_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input annotations_

**Name in Workflow File:** in-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_

And 1 _output port_:

**Name in GUI:** _Result annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
