---
title: "Insert Restriction Site"
weight: 100
---

# Insert Restriction Site

To open the _Insert Restriction Site_ dialog, use the _Edit ‣ Insert Restriction Site_ option from the sequence editing section in the _Actions_ main menu or in the context menu of the _Sequence View_, or press the Ctrl-Shift-I keys:

![](/images/113541166/113541169.png)

Select an enzyme whose site sequence you want to paste into the entire sequence in the "Choose site to paste" field.

The "Show sites with undefined suppliers" button makes visible all restriction enzymes available. When it is unchecked (default), only enzymes that have at least one supplier are available.

You can also configure how annotations located in an edited region should be modified.

Select one of the following in the _Annotation region resolving_ mode:

* _Expand affected annotation with position to insert_ — if an annotation is located in an edited region, it is expanded in case of character insertion.
* _Remove affected annotation_ — all annotations in an edited region are removed.
* _Split (join annotation parts)_ — an annotation is split into two joined elements (see "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details).
* _Split (separate annotation parts)_ — an annotation is split into two separate parts.

You can also check the _Recalculate values of qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed during sequence editing. Qualifier values that specify coordinates (like "100..200") are recalculated according to the sequence modification. For example, the value might become "104..204" if four characters have been inserted before the corresponding annotation.

You can also select the _Save to new file_ checkbox to save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select the _Merge annotation in this file_ option.