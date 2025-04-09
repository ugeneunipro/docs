---
title: "Insert subsequence"
weight: 200
---


# Insert subsequence

To open the _Insert sequence_ dialog use the _Edit ‣ Insert subsequence_ on sequence editing in th_e Actions_ main menu or in the context menu of the _Sequence View_ or press the Ctrl-I key:


![](/images/96665661/96665671.png)

Insert a sequence in the _Paste data here_ field.

You can also configure the way how annotations located in an edited region should be modified.

Select one of the following in the _Annotation region resolving_ mode:

*   _Expand affected annotation with position to insert_ — an annotation located in an edited region is expanded in case of characters insertion.
*   _Remove affected annotation_ — all annotations in an edited region are removed.
*   _Split (join annotation parts)_ —  an annotation is split into two join elements (see "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details).
*   _Split (separate annotation parts)_ — an annotation is split into two.

It is also possible to check the _Recalculate values of qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed on the sequence editing. Qualifiers values that specify coordinates (like "100..200") are re-calculated accordingly to the sequence modification. For example, the value might become "104..204", if four characters have been inserted before the corresponding annotation.

You can also select _Save to new file_ checkbox and save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select _Merge annotation in this file_ option.
