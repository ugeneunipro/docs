---
title: "Editing Sequence"
weight: 1
---


# Editing Sequence

If the corresponding document is not locked, it is possible to edit a sequence.

### Editing mode and annotations settings

To switch on the editing mode for the sequence, select the _Edit sequence_ button on the left toolbar of the _Details View_:


![](/images/65929426/65929427.png)

A special cursor appears in this case, and the sequence can be edited as in a text editor:

*   To insert characters to the sequence, move the cursor to the required location and type the characters or paste them using _Ctrl + V_ / _Cmd + V_ keyboard shortcut.
*   To replace a sequence region, select it and insert the new characters.
*   To remove a character from the sequence, move the cursor to the required location and press _Backspace_ or _Delete_. To remove a region, select it and press one of these shortcuts.

One can also configure the way how annotations located in an edited region should be modified. To open a dialog with the settings select _Edit–>Annotations settings on sequence editing_ in th_e Actions_ main menu or in the context menu of the _Sequence View_.


![](/images/65929426/65929428.png)

Select one of the following:

*   _Expand or crop affected annotation_ — an annotation located in an edited region is expanded in case of characters insertion or cropped in case of characters deletion.
*   _Remove affected annotation_ — all annotations in an edited region are removed.
*   _Split (join annotation parts)_ —  an annotation is split into two join elements (see "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details).
*   _Split (separate annotation parts)_ — an annotation is split into two annotations.

It is also possible to check the _Recalculate values of qualifiers_ option in the dialog. If it is selected, qualifiers of all annotations are parsed on the sequence editing. Qualifiers values that specify coordinates (like "100..200") are re-calculated accordingly to the sequence modification. For example, the value might become "104..204", if four characters have been inserted before the corresponding annotation.

### Getting reverse-complement, reverse, or complement sequence

To replace a sequence with its reverse-complement sequence, select _E__dit–>Reverse-complement sequence_ in th_e Actions_ main menu or in the context menu of the Sequence View. The keyboard shortcut for this action is _Ctrl + Shift + R_ / _Cmd + Shift + R_.

Use the _Reverse sequence_ or _Complement _sequence__ items in the same menus to replace the sequence with its reverse or complement sequence.
