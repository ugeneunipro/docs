---
title: "MUSCLE Aligning"
weight: 100
---

# MUSCLE Aligning

To run the classic MUSCLE, use the _Align ‣ Align with MUSCLE_ context menu item in the _Alignment Editor_.

![](/images/65930833/65930834.png)

The dialog contains a list of MUSCLE modes: _MUSCLE default_, _Large alignment_, _Refine only_.

![](/images/65930833/65930835.png)

By default, UGENE does not rearrange the sequence order in an alignment, but the original MUSCLE package does. To enable sequence rearrangement, uncheck the _Do not re-arrange sequences (-stable)_ option in the dialog.

One of the improvements to the original MUSCLE package is the ability to align only a part of the model. When the _Column range_ item is selected, the region of the specified columns is only passed to the MUSCLE alignment engine. The resulting alignment is inserted into the original one with gaps added or removed at the region boundaries.

To visually select the column range to align, make a selection in the alignment editor first. Then invoke the MUSCLE plugin. Its column range boundary values will automatically match the given selection.