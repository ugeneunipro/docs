---
title: "Insert Subsequence"
weight: 200
---

# Insert Subsequence

To open the _Insert Sequence_ dialog, use the _Edit ‣ Insert Subsequence_ option in the sequence editing section of the _Actions_ main menu or in the context menu of the _Sequence View_, or simply press the Ctrl-I key:

![](/images/96665661/96665671.png)

Insert a sequence in the _Paste Data Here_ field.

You can also configure how annotations located in the edited region should be modified.

Select one of the following options in the _Annotation Region Resolving_ mode:

*   _Expand affected annotation with position to insert_ — an annotation located in an edited region is expanded in case of character insertion.
*   _Remove affected annotation_ — all annotations in an edited region are removed.
*   _Split (join annotation parts)_ — an annotation is split into two joined elements (see "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details).
*   _Split (separate annotation parts)_ — an annotation is split into two separate parts.

It is also possible to check the _Recalculate Values of Qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed during sequence editing. Qualifiers with values that specify coordinates (like "100..200") are recalculated in accordance with the sequence modification. For example, the value might become "104..204" if four characters have been inserted before the corresponding annotation.

You can also select the _Save to New File_ checkbox to save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select the _Merge Annotation in This File_ option.