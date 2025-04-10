---
title: "Saving Graph Cutoffs as Annotations"
weight: 300
---

# Saving Graph Cutoffs as Annotations

To save graph cutoffs as annotations, select the _Graph->Save cutoffs as annotations_ item in the graph context menu. The following dialog will appear:

![](/images/65929579/65929580.png)

The following parameters are available:

- _Maximum cutoff_ - maximum cutoff value.
- _Minimum cutoff_ - minimum cutoff value.
- _Around cutoff values_ - saves the values around cutoff values.
- _Between cutoff values_ - saves the values between cutoff values.

In the _Save annotation(s) to_ group, you can set up a file to store annotations. It could be either an existing annotation table object, a new annotation table, or an auto-annotations table (if it is available).

In the _Annotation parameters_ group, you can specify the name of the group and the name of the annotation. If the group name is set to `<auto>`, UGENE will use the group name as the name for the group. You can use the ‘/’ character in this field as a group name separator to create subgroups. If the annotation name is set to _by type_, UGENE will use the annotation type from the _Annotation type:_ table as the name for the annotation. You can also add a description in the corresponding text field.

Select the parameters and click on the _Save_ button. The corresponding annotations will be saved.