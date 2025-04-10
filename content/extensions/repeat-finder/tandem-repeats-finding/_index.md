---
title: "Tandem Repeats Finding"
weight: 200
---

# Tandem Repeats Finding

To find tandem repeats, select the _Analyze ‣ Find tandem repeats..._ context menu item in the _Sequence View_ window.

In the opened dialog, you can specify the tandem search parameters, the region to search in, and the result parameters:

![](/images/65930740/65930741.png)

The dialog parameters:

- _Present Settings_ — Specify the tandem repeats parameters with predefined values by selecting an available preset.
- _Algorithm_ — This parameter allows you to select the search algorithm. The default and fast option is the optimized suffix array algorithm.
- _Min length of repeated sequence_ — The minimum acceptable repeat length measured in base symbols.
- _Max length of repeated sequence_ — The maximum acceptable repeat length measured in base symbols.
- _Min length of tandem repeat_ — The minimum tandem size sets the limit on the minimum acceptable length of the tandem, i.e., the minimum total repeat length of the searched tandem.
- _Min number of repeats_ — The minimum number of repeats of a searched tandem.
- _Show overlapped tandems_ — Check if the plugin should search for overlapped tandems; otherwise, keep it unchecked.
- _Search in_ — Specify the region to search in: the whole sequence, a custom region, or the region of the current selection (if any).

The output settings can be found in the _Output_ tab:

In the _Save annotation(s) to_ group, you can set up a file to store annotations. It could be an existing annotation table object, a new annotation table, or an auto-annotations table (if available).

In the _Annotation parameters_ group, you can specify the name of the group and the name of the annotation. If the group name is set to `<auto>`, UGENE will use the group name as the name for the group. You can use the ‘/’ character in this field as a group name separator to create subgroups. If the annotation name is set to _by type_, UGENE will use the annotation type from the _Annotation type:_ table as the name for the annotation. Also, you can add a description in the corresponding text field.