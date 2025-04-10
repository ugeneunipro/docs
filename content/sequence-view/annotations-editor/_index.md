---
title: "Annotations Editor"
weight: 900
---

# Annotations Editor

The _Annotations Editor_ contains tools to manipulate annotations for a sequence. It provides a convenient way to organize, view, and modify a single annotation as well as annotation groups.

An annotation for a sequence consists of:

*   _Name_ (or key) — indicates the biological nature of the annotated feature.
*   _Location_ — coordinates in the sequence.
*   _The list of qualifiers_ — qualifiers are the general mechanism for supplying information about annotations. Qualifiers are stored as pairs of (name, value) strings.

Below is the default layout of the _Annotations Editor_ with an extra column for the “note” qualifier added:

![](/images/65929451/65929452.png)

There are usually several objects with annotations in the _Annotations Editor_. A special _Auto-annotations_ object is always present for each sequence opened. It contains annotations automatically calculated for the sequence (see [below](http://ugene.unipro.ru/documentation/manual/sequence_view/annotations_editor.html#auto-annotations) for details).

An object contains groups of annotations used by UGENE for the logical organization of the annotations. An annotation must always belong to some group.

For documents created not by UGENE, annotations are grouped by their names. For annotations created in UGENE, it is possible to use arbitrary group names.

Groups can contain both annotations and other groups. The numbers in the brackets after a group name in the _Annotations Editor_ indicate the count of subgroups and annotations in the current group.

A single annotation is allowed to be presented in several groups simultaneously. An annotation is physically removed from the document when it does not belong to any group.