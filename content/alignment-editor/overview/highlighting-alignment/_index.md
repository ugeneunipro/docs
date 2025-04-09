---
title: "Highlighting Alignment"
weight: 500
---


# Highlighting Alignment

To apply an alignment highlighting mode, select it in the _Highlighting_ context menu:

![](/images/65929627/96666024.png)

or on the _Highlighting_ tab of the _Options Panel:_

![](/images/65929627/96666026.png)

### Referense sequence

Some highlighting algorithms consider not the alignment itself, but changes of the whole alignment (minus one sequence) from one sequence. This one sequence is called the reference sequence and you may set it here.

**NOTE**: not all highlighting algorithms take the reference into account, those that do that will be marked **RS** below.

### Color

Different color schemes. Pay attention, that DNA and AMINO alignment have different color schemes:

*   _No colors_ - no colors at all.

The list of Jalview compatible color schemes for amino acid alphabet only:

*   _Buried Index_,
*   _Turn propensity_,
*   _Strand propensity_,
*   _Helix propensity_,
*   _Hydrophobicity_,
*   _Tailor_,
*   _Zappo_.

Look at the following table for the color details:

![](/images/65929627/96666029.png)The list of DNA/RNA/amino alphabet color schemes:

*   _Percentage identity_ - the higher the frequency percentage value of the base in the certain column, the bluer the corresponding base (only the highest frequency base is colored),
*   _Percentage identity (gray)_ - the same as _Percentage identity_, but in black and white,
*   _UGENE_ (**default**) - classic UGENE color scheme,
*   _UGENE Sanger_ - UGENE color scheme, which is mainly used in the Sanger Reads editor,
*   _Weak similarities_ - look [here](https://ugene.dev/tracker/browse/UGENE-6548) for details.

The list of DNA/RNA alphabet color schemes:

*   _Jalview_ - Jalview compatible color scheme,
*   _Percentage identity (colored)_ - look [here](https://ugene.dev/tracker/browse/UGENE-6474) for details.

### Highlighting

Choose, what types of bases will be colored with the color scheme choosen. The following modes are available:

*   _Agreements_ (**RS**) — highlights symbols that coincide with the reference sequence.

*   _Disagreements_ (_**RS**)_ — highlights symbols that differ from the reference sequence.

*   _Gaps_ - highlights gaps only.
*   _Conservation level_ - highlights bases, which frequency percentage value of the column is greater/lower, than the corresponding threshold.
*   _Transitions (**RS**)_ - highlights transitions of the referense base. Transitions are interchanges of two-ring purines (A <-> G), or of one-ring pyrimidines (C <-> T): they therefore involve bases of similar shape.
*   _Transversions (**RS**)_ - highlights transversions of the referense base. Transversions are interchanges of purine for pyrimidine bases, which therefore involve exchange of one-ring & two-ring structures.

Look at the following pictures for details about transitions and transversions:
![Transitions and transversions](/images/65929627/96666031.png "Transitions and transversions")

To use dots instead of symbols which are not highlighted check the _Use dots_ checkbox.

### _Export highlighted_

Also you can export highlighting with a help of the _Export_ button in the _Options Panel_ or by the _Export->Export highlighted_ context menu item. Check the corresponding page fpr details.
