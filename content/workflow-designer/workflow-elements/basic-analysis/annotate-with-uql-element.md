---
title: "Annotate with UQL Element"
weight: 200
---

# Annotate with UQL Element

Analyzes a nucleotide sequence with a UGENE Query Language (UQL) workflow. The workflow specifies a set of features to
search for and their positional relationship.

To learn more about UQL workflows
read [UGENE Query Designer Manual](https://doc.ugene.net/wiki/display/UM/About+the+Query+Designer).

**Element type:** query

## Parameters

| Parameter               | Description                                                                                                       | Default value | Parameter in Workflow File | Type      |
|-------------------------|-------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Workflow** (required) | UQL workflow file.                                                                                                |               | **schema**                 | _string_  |
| **Merge**               | Merges regions of each result into a single annotation.                                                           | False         | **merge**                  | _boolean_ |
| **Offset**              | If the _Merge_ parameter is set to _True_, adds left and right offsets of the specified length to the annotation. | 0             | **offset**                 | _numeric_ |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input sequences_
**Name in Workflow File:** in-sequence
**Slots:**

| Slot In GUI  | Slot in Workflow File | Type       |
|--------------|-----------------------|------------|
| **Sequence** | **sequence**          | _sequence_ |

And 1 _output port_:

**Name in GUI:** _Result annotations_
**Name in Workflow File:** out-annotations
**Slots:**

| Slot In GUI            | Slot in Workflow File | Type               |
|------------------------|-----------------------|--------------------|
| **Set of annotations** | **annotations**       | _annotation-table_ |
