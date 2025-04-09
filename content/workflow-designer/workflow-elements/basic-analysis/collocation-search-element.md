---
title: "Collocation Search Element"
weight: 400
---


# Collocation Search Element

Finds groups of specified annotations in each supplied set of annotations, stores found regions as annotations.

**Element type:** collocated-annotation-search

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Result type**

Copy original annotations or annotate found regions with new ones.

Create new annotations

**result-type**

_string_

**Result annotation** (required)

Name of the result annotation to mark found collocations.

misc\_feature

**result-name**

_string_

**Include boundaries**

Include most left and most right boundary annotations regions into result or exclude them.

True

**annotations**

_string_

**Group of annotations** (required)

List of annotation names to search. Found regions will contain all the named annotations.



**include-boundary**

_boolean_

**Region size**

Effectively this is the maximum allowed distance between the interesting annotations in a group.

1000

**region-size**

_numeric_

**Must fit into region**

Specifies whether the interesting annotations should entirely fit into the specified region to form a group.

False

**must-fit**

_boolean_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input data_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

**Set of annotations**

**annotations**

_annotation-table-list_

And 1 _output port_:

**Name in GUI:** _Group annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
