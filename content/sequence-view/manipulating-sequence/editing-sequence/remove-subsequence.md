---
title: "Remove subsequence"
weight: 1
---


# Remove subsequence

To open the _Remove subsequence_ dialog use the _Edit ‣ Remove subsequence_ on sequence editing in th_e Actions_ main menu or in the context menu of the _Sequence View._


![](/images/96665657/96665688.png)

Correct value in the _Remove region_ option. By default it displays the beginning and end of the sequence.

You can also configure the way how annotations located in an edited region should be modified.

Select one of the following in the _Annotation region resolving_ mode:

*   _Crop corresponding annotation_ — an annotation located in an edited region is cropped.
*   _Remove corresponding annotation_ — all annotations in an edited region are removed.

It is also possible to check the _Recalculate values of qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed on the sequence editing. Qualifiers values that specify coordinates (like "100..200") are re-calculated accordingly to the sequence modification. For example, the value might become "104..204", if four characters have been inserted before the corresponding annotation.

You can also select _Save to new file_ checkbox and save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select _Merge annotation in this file_ option.
