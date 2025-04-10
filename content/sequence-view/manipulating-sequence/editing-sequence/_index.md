---
title: "Editing Sequence"
weight: 900
---

# Editing Sequence

If the corresponding document is not locked, it is possible to edit a sequence.

### Editing Mode and Annotation Settings

To switch to the editing mode for the sequence, select the _Edit Sequence_ button on the left toolbar of the _Details View_:

![](/images/65929426/65929427.png)

A special cursor will appear, allowing you to edit the sequence as in a text editor:

- To insert characters into the sequence, move the cursor to the desired location and type the characters or paste them using the _Ctrl + V_ / _Cmd + V_ keyboard shortcut.
- To replace a sequence region, select it and insert the new characters.
- To remove a character from the sequence, move the cursor to the required location and press _Backspace_ or _Delete_. To remove a region, select it and press one of these shortcuts.

You can also configure how annotations located in an edited region should be modified. To open a dialog with the settings, select _Edit–>Annotations settings on sequence editing_ in the _Actions_ main menu or in the context menu of the _Sequence View_:

![](/images/65929426/65929428.png)

Select one of the following:

- _Expand or crop affected annotation_ — an annotation located in an edited region is expanded in case of character insertion or cropped in case of character deletion.
- _Remove affected annotation_ — all annotations in an edited region are removed.
- _Split (join annotation parts)_ — an annotation is split into two joined elements (see "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details).
- _Split (separate annotation parts)_ — an annotation is split into two separate annotations.

It is also possible to check the _Recalculate values of qualifiers_ option in the dialog. If it is selected, qualifiers of all annotations are parsed during sequence editing. Qualifier values that specify coordinates (like "100..200") are recalculated according to the sequence modification. For example, the value might become "104..204" if four characters have been inserted before the corresponding annotation.

### Getting Reverse-Complement, Reverse, or Complement Sequence

To replace a sequence with its reverse-complement sequence, select _Edit–>Reverse-complement sequence_ in the _Actions_ main menu or in the context menu of the Sequence View. The keyboard shortcut for this action is _Ctrl + Shift + R_ / _Cmd + Shift + R_.

Use the _Reverse sequence_ or _Complement sequence_ items in the same menus to replace the sequence with its reverse or complement sequence.