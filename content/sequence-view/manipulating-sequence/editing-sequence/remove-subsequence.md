---
title: "Remove Subsequence"
weight: 300
---

# Remove Subsequence

To open the _Remove Subsequence_ dialog, use the _Edit ‣ Remove Subsequence_ option in the sequence editing section of the _Actions_ main menu or in the context menu of the _Sequence View_.

![](/images/96665657/96665688.png)

Correct the value in the _Remove Region_ option. By default, it displays the beginning and end of the sequence.

You can also configure how annotations located in an edited region should be modified.

Select one of the following in the _Annotation Region Resolving_ mode:

*   _Crop corresponding annotation_ — an annotation located in an edited region is cropped.
*   _Remove corresponding annotation_ — all annotations in an edited region are removed.

It is also possible to check the _Recalculate Values of Qualifiers_ option in the dialog. If selected, all annotations' qualifiers are parsed during sequence editing. Qualifier values that specify coordinates (like "100..200") are recalculated according to the sequence modification. For example, the value might become "104..204" if four characters have been inserted before the corresponding annotation.

You can also select the _Save to New File_ checkbox and save the modified sequence to a new file by specifying the format and location of the document.

It is also possible to select the _Merge Annotation in This File_ option.