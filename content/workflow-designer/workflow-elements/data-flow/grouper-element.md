---
title: "Grouper Element"
weight: 200
---


# Grouper Element

The element groups data supplied to the specified slot by the specified property (for example, by value). Additionally, it is possible to merge data from another slots associated with the specified one.

**Element type:** grouper

Parameters
----------

To use the _Grouper_ element connect the _Grouper’s_ input port to the required workflow element. Select the _Grouper_ element on the _Scene_ and specify _Group slot_ and _Group operation_ parameters in the _Parameters_ area in the _Property Editor_. To merge associated data, it is possible to create as many _Output slot(s)_ as required (see details below).

### Group slot

The _Group slot_ specifies a _slot_ that is used to group the input data. The list of available values of the parameter depend on the slots of workflow elements which produce data in the workflow before the _Grouper_ element. There is a special _Unset_ value. When it is selected, only one group is created.

### Group operation

The _Group operation_ specifies criteria to group data supplied to the _Group slot_. It can take the following values:

*   _By value_ - input data are compared by value (a group is created for each unique value, it can contain one or several identical values)
*   _By identity_ - input data are compared by internal data ID (all values are unique)
*   _By name_ - input data are compared by their names

_By value_ group operation is available for group slots of types _Sequence_, _Set of annotations_, _MSA_, _Plain text_, _Source URL_. _By identity_ and _By name_ group operations are available for group slots of type _Sequence_ only.

### Output slots

When data supplied to the _Group slot_ are divided into different groups the associated data are also got into a group. The possible associated data depend on the workflow. For example, a [_Sequence Reader_](../data-readers/read-sequence-element) element contains slots _Sequence_ and _Set of annotations_. These data are **associated** as annotations belong to a sequence. Another example of associated data are sequence markers created by the _[Sequence Marker](sequence-marker-element)_ element. The associated data, therefore, can be additionally handled (i.e. merged) by the _Grouper_element. The action that can be performed on the associated data depends on their type. In any case to output handled associated data you need to create a new output slot in the_Grouper_ element. To create it click the _Add_ button in the _Grouper’s Parameters_ area. The following dialog appears:

![](/images/65930076/65930077.png)

In the dialog you should select a _Source data slot_ (i.e. a slot with the associated data) and input a name of the new slot. Click the OK button. A new dialog appears that specifies how the associated data should be merged. The view of the dialog and the available merge actions for different types of the _Source data slot_ are the following:

*   For a _Set of annotations_ slot the _New Annotations Action_ dialog appears:

![](/images/65930076/65930078.png)

You can merge annotations into one annotation table and, optionally, filter duplicated annotations. Also, you can shift annotations. To do it, you need to create another output slot with type _Sequence_ and _Merge into one sequence_ option selected (see below). In other words you need to merge all sequences in a group into one sequence. In this case you select the corresponding sequence slot in the _New Annotations Action_ dialog and each set of annotations in a group is shifted according to the corresponding sequence in the group. As the result you have one sequence and one set of annotations allocated on the whole sequence.

*   For _Source URL_ and _Plain text_ slots the _New String Action_ dialog appears:

![](/images/65930076/65930079.png)

Using this dialog you can merge strings into one string. Optionally, you can specify an additional strings separator.

*   For a _Sequence_ slot the _New Sequence Action_ dialog appears:

![](/images/65930076/65930080.png)

You can either merge all sequences in a group into one sequence or create a multiple sequence alignment. In the first case you need to specify the _Merged sequence name_ and you can select the number of unknown characters between the merged sequences. In the second case you need to specify the alignment name. To filter duplicated sequence check the corresponding check box.

*   For a _MSA_ slot the _New Alignment Action_ dialog appears:

![](/images/65930076/65930081.png)

Input the alignment name in this dialog. To filter duplicated rows check the corresponding check box.

To edit a created slot, select it in the _Parameters_ area of the _Grouper_ element and click the _Edit_ button. To remove the slot, select it and click the _Remove_ button.

Input/Output Ports
------------------

The element has 1 _input port_ that can take any incoming data.

**Name in GUI:** _Input data flow_

**Name in workflow File:** input-data

The element has 1 _output port_.

**Name in GUI:** _Grouped output data flow_

**Name in workflow File:** output-data

**Slots:**

Slot In GUI

Slot in workflow File

Type

**Group size**

**group-size**

_string_

Also the port has one default slot of the grouped data and it may also have one or several customized output slots (see above).
