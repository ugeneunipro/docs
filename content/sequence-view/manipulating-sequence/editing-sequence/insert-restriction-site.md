---
title: "Insert Restriction Site"
weight: 1
---


# Insert Restriction Site

To open the _Insert Restriction SIte_ dialog use the _Edit ‣ Insert _Restriction SIte__on sequence editing in th_e Actions_ main menu or in the context menu of the _Sequence View_ or press the Ctrl-Shift-I key:

![](/images/113541166/113541169.png)

Select an enzyme, which site sequence you want to paste to the whole sequence in the "Choose site to paste" field.

The "Show sites with undefined suppliers" button makes visible all resriction enzimes avaliable. When it is unchecked (default) only enzymes, which have at leas one supplier, are available.

You can also configure the way how annotations located in an edited region should be modified.



Select one of the following in the _Annotation region resolving_ mode:

*   _Expand affected annotation with position to insert_ — an annotation located in an edited region is expanded in case of characters insertion.
*   _Remove affected annotation_ — all annotations in an edited region are removed.
*   _Split (join annotation parts)_ —  an annotation is split into two join elements (see "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details).
*   _Split (separate annotation parts)_ — an annotation is split into two.

It is also possible to check the _Recalculate values of qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed on the sequence editing. Qualifiers values that specify coordinates (like "100..200") are re-calculated accordingly to the sequence modification. For example, the value might become "104..204", if four characters have been inserted before the corresponding annotation.

You can also select _Save to new file_ checkbox and save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select _Merge annotation in this file_ option.
