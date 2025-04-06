---
title: "Find Repeats Element"
weight: 1
---


# Find Repeats Element

Finds repeats in each supplied sequence, stores found regions as annotations.

**Element type:** repeats-search

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Annotate as** (required)

Name of the result annotation to mark found repeats.

repeat\_unit

**result-name**

_string_

**Algorithm**

Control over variations of the algorithm.

Auto

**algorithm**

_numeric_

Available values are:

*   0 - algorithm choosed automaticly
*   1 - for diagonal algorithm
*   2 - for suffix index algorithm

**Filter nested**

Filters nested repeats.

True

**filter-nested**

_boolean_

**Identity**

Repeats identity in percent.

100

**identity**

_numeric_

**Inverted**

Specifies to search for inverted repeats.

False

**inverted**

_boolean_

**Max distance**

Maximum distance between the repeats.

5000

**max-distance**

_numeric_

**Min distance**

Minimum distance between the repeats.

0

**min-distance**

_numeric_

**Min length**

Minimum length of the repeats.

5

**min-length**

_numeric_

**Parallel threads**

Number of parallel threads used for the task.

Auto

**threads**

_numeric_

0 - for using autodetected threads number



Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input sequence_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

And 1 _output port_:

**Name in GUI:** _Repeat annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
