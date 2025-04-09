---
title: "Running Schema from the Sequence View"
weight: 500
---


# Running Schema from the Sequence View

Prepare a query _schema_ and [_save_](manipulating-schema/saving-schema) it to a file.

Open a nucleotide sequence that you want to analyze with this query schema. You can see the sequence displayed in the **Sequence view**.

To learn more about the **Sequence view** read the main UGENE User Manual.

Select the _Analyze ‣ Analyze with Query Schema_ item in the _Actions_ main menu or in the context menu:


![](/images/65930656/65930657.png)

The _Analyze with query schema_ dialog appears:


![](/images/65930656/65930658.png)

Browse for the file with a query schema. The selected schema preview appears in the dialog, for example:


![](/images/65930656/65930659.png)

You can also adjust other parameters:

_Region_ — the sequence range to analyze with the query schema, you can select:

*   *   _Whole sequence_ — to analyze the whole sequence.
    *   _Selected range_ — to analyze the currently selected sequence region. This item is disabled if there is no region selected.
    *   _Custom range_ — to specify manually a range to analyze.

In the _Save annotation(s) to_ group you can set up a file to store annotations.  It could be either an existing annotation table object, a new annotation table or auto-annotations table (if it is available).

In the _Annotation parameters_ group you can specify the name of the group. If the group name is set to <auto> UGENE will use the group name as the name for the group. Also you can add a description in the corresponding text field.
