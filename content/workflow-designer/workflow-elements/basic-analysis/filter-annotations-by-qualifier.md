---
title: "Filter Annotations by Qualifier"
weight: 1
---


# Filter Annotations by Qualifier

Filters annotations by qualifier.

**Element type:** filter-annotations-by-qualifier

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Qualifier name**

Name of the qualifier to use for filtering.



**qualifier-name**

_string_

**Qualifier value**

Text value of the qualifier to apply as filtering criteria.



**qualifier-value**

_string_

**Accept or filter**

Selects the name filter: accept specified names or accept all except specified.

True

**accept-or-filter**

_boolean_

Input/Output Ports
------------------

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
