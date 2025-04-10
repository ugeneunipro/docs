---
title: "Replace Subsequence"
weight: 400
---

# Replace Subsequence

To open the _Replace Subsequence_ dialog, use the _Edit ‣ Replace Subsequence_ option in the sequence editing section of the _Actions_ main menu or in the context menu of the _Sequence View_, or press the Ctrl-R key.

Note that the part of the sequence you want to replace must be selected; otherwise, the menu item will not be available.

![](/images/96665651/96665697.png)

The selected part of the sequence will appear in the _Paste data here_ field.

You can also configure how annotations located in the edited region should be modified.

Select one of the following in the _Annotation Region Resolving_ mode:

*   _Expand Affected Annotation_ — An annotation located in the edited region is replaced in case of character insertion.
*   _Remove Affected Annotation_ — All annotations in the edited region are removed.

You can also choose to check the _Recalculate Values of Qualifiers_ option in the dialog. If selected, all annotations' qualifiers will be parsed during sequence editing. Qualifier values that specify coordinates (like "100..200") are recalculated according to the sequence modification. For example, the value might become "104..204" if four characters have been inserted before the corresponding annotation.

You can also select the _Save to New File_ checkbox to save the modified sequence to a new file by specifying the document's format and location.

It is also possible to select the _Merge Annotation in This File_ option.