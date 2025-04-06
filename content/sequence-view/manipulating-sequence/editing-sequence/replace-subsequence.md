---
title: "Replace subsequence"
weight: 1
---


# Replace subsequence

To open the _Replace sequence_ dialog use the _Edit ‣ Replace subsequence_ on sequence editing in th_e Actions_ main menu or in the context menu of the _Sequence View_ or press the Ctrl-R key:

Note, that the part of the sequence that you are going to replace must be selected, otherwise the menu item is not available.


![](/images/96665651/96665697.png)

Selected part of sequence is in the _Paste data here_ field.

You can also configure the way how annotations located in an edited region should be modified.

Select one of the following in the _Annotation region resolving_ mode:

*   _Expand affected annotation_  — an annotation located in an edited region is replaced in case of characters insertion.
*   _Remove affected annotation_ — all annotations in an edited region are removed.

It is also possible to check the _Recalculate values of qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed on the sequence editing. Qualifiers values that specify coordinates (like "100..200") are re-calculated accordingly to the sequence modification. For example, the value might become "104..204", if four characters have been inserted before the corresponding annotation.

You can also select _Save to new file_ checkbox and save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select _Merge annotation in this file_ option.
