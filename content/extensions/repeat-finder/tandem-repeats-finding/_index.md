---
title: "Tandem Repeats Finding"
weight: 200
---


# Tandem Repeats Finding

To find tandem repeats, select the _Analyze ‣ Find tandem repeats..._ context menu item in the _Sequence View_ window.

In the opened dialog you can specify the tandem search parameters, the region to search in and the result parameters:


![](/images/65930740/65930741.png)

The dialog parameters:

_Present Settings_ — specify the tandem repeats parameters with predefined values by selecting the available preset.

_Algorithm_ — the algorithm parameter allows to select the search algorithm. The default and a fast one is optimized suffix array algorithm.

_Min length of repeated sequence -_ the minimum acceptable repeat length measured in base symbols.

_Max length of repeated sequence -_ the maximum acceptable repeat length measured in base symbols.

_Min length of tandem repeat -_ the minimum tandem size sets the limit on the minimum acceptable length of the tandem, i.e. the minimum total repeats length of the searched tandem.

_Min number of repeats -_ the minimum number of repeats of a searched tandem.

_Show overlapped tandems -_ check if the plugin should search for the overlapped tandems, otherwise keep unchecked.

_Search in -_ specify the region to search in the whole sequence, a custom region or the region of the current selection (if any).

The output settings can be found in the _Output_ tab:

In the _Save annotation(s) to_ group, you can set up a file to store annotations.  It could be either an existing annotation table object, a new annotation table or auto-annotations table (if it is available).

In the _Annotation parameters_ group, you can specify the name of the group and the name of the annotation. If the group name is set to <auto> UGENE will use the group name as the name for the group. You can use the ‘/’ characters in this field as a group name separator to create subgroups. If the annotation name is set to _by type_ UGENE will use the annotation type from the _Annotation type:_ table as the name for the annotation. Also, you can add a description in the corresponding text field.
