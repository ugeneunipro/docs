---
title: "Sequence Marker Element"
weight: 400
---

# Sequence Marker Element

This element adds one or several marks to the input sequence depending on its properties. Use this element, for example, in conjunction with the [_Filter_](filter-element) element.

**Element Type:** mark-sequence

## Parameters

To create a new marker group that marks the input sequence, click the _Add_ button in the _Parameters_ area. The _Create Marker Group_ dialog will appear:

![](/images/65930090/65930091.png)

Choose a type for the marker group and input a marker group name. The following types are available:

- _Length markers_ — marks a sequence based on its length. The sequence is marked if its length is less or greater than the specified value.
- _Sequence name markers_ — marks a sequence based on its name.
- _Annotations count markers_ — marks a sequence based on the number of annotations.
- _Qualifier integer value markers_ — marks a sequence based on the number of integer qualifiers.
- _Qualifier text value markers_ — marks a sequence based on the number of text qualifiers.
- _Qualifier float value markers_ — marks a sequence based on the number of float qualifiers.
- _Text markers_ — marks a sequence based on a file name. For example, if the name:
  1. starts with the specified text;
  2. ends with the specified text;
  3. contains the specified text;
  4. matches the specified regular expression.

Each marker group can contain more than one marker. Use the _Add_, _Edit_, and _Remove_ buttons in the dialog to create, modify, and delete markers in the marker group.

To edit a created marker group, select the group in the _Parameters_ area and click _Edit_:

![](/images/2097367/2359347.png)

To remove a marker group, select it in the list and click _Remove_.

## Input/Output Ports

The element has one _input port_:

| **Name in GUI** | **Name in Workflow File** | **Type**               |
|-----------------|---------------------------|------------------------|
| _Sequence_      | in-sequence               | _sequence_             |
| _Location_      | url                       | _string_               |
| _Set of annotations_ | annotations           | _annotation-table-list_ |

The element has one _output port_:

| **Name in GUI**     | **Name in Workflow File** | **Type** |
|---------------------|---------------------------|----------|
| _Marked sequence_   | out-marked-seq            | Each created marker group adds a text slot with the following properties: |
| Name of the marker group | Name of the marker group | _string_ |

