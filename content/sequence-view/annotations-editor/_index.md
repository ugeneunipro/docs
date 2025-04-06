---
title: "Annotations Editor"
weight: 1
---


# Annotations Editor

The _Annotations editor_ contains tools to manipulate annotations for a sequence. It provides a convenient way to organize, view and modify a single annotation as well as annotation groups.

An annotation for a sequence consists of:

*   _Name_ (or key) — indicates the biological nature of the annotated feature.
*   _Location_ — coordinates in the sequence.
*   _The list of qualifiers_ — qualifiers are the general mechanism for supplying information about annotation. Qualifiers are stored as pairs of (name, value) strings.

Below is the default layout of the _Annotations editor_ with an extra column for the “note” qualifier added:


![](/images/65929451/65929452.png)

There are usually several objects with annotations in the _Annotations editor_. A special _Auto-annotations_ object is always presented for each sequnce opened. It contains annotations automatically calculated for the sequence (see [_below_](http://ugene.unipro.ru/documentation/manual/sequence_view/annotations_editor.html#auto-annotations) for details).

An object contains groups of annotations used by UGENE for logical organization of the annotations. An annotation must always belongs to some group.

For documents created not by UGENE annotations are grouped by their names. For annotations created in UGENE it is possible to use arbitrary group names.

Groups can contain both annotations and other groups. The numbers in the brackets after a group name in the _Annotations editor_ are the count of subgroups and annotations in the current group.

A single annotation is allowed to be presented in several groups simultaneously. An annotation is physically removed from the document when it does not belong to any group.

*   [Automatic Annotations Highlighting](automatic-annotations-highlighting.md)
*   [db\_xref Qualifier](db_xref-qualifier.md)
*   [The comment Annotation](the-comment-annotation.md)
*   [Transform into a primer pair](transform-into-a-primer-pair.md)


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
