---
title: "How to Create and Run Schema"
weight: 300
---


# How to Create and Run Schema

*   Select the _Tools ‣ Query Designer_ item in the main menu.

**Result:** The Query Designer window appears:


![](/images/65930610/65930611.png)

*   Drag the _Repeats_ element from the _Palette_ to the _Scene_.

**Result:** The _Repeats_ element subunits are presented on the _Scene_:


![](/images/65930610/65930612.png)

Note, that by default minimum distance between left and right repeats is 0bp, the maximum distance is 5000bp.

*   Slide the _Repeats_ element subunits apart.

**Result:**


![](/images/65930610/65930613.png)

*   Drag the _ORF_ element from the _Palette_ and drop it between the repeats.

**Result:** The _ORF_ element is presented on the _Scene_:


![](/images/65930610/65930614.png)

*   Find the _End-Start_ constraint on the _Palette_:


![](/images/65930610/65930615.png)

And drag it between the left _Repeats_ element and _ORF_.

**Result:** The dialog appears:


![](/images/65930610/65930616.png)

*   Check that _From_ equals to _Repeats.left_ and _To_ equals to _ORF_. Set _Max_ to 5000. Press the _OK_ button.

**Result:** The constraint has been added to the elements:


![](/images/65930610/65930617.png)

*   Repeat steps 5-6 for _ORF_ element and the right _Repeats_ subunit.

**Result:** The schema looks as follows:


![](/images/65930610/65930618.png)

*   Press the _Run Schema_ button on the toolbar:


![](/images/65930610/65930619.png)

**Result:** The _Run schema_ dialog appears:


![](/images/65930610/65930620.png)

*   Browse for the sequence to analyze (the _Load sequence_ field) and for a GenBank file to save results to (the _Save results to_ field). Click the _Run_ button.

**Result:** Both the sequence and the file with annotations are added to the current project. The sequence appears in the Sequence View window, for example:


![](/images/65930610/65930621.png)

To learn more about the Sequence View read main UGENE User Manual.

The schema described in this example is also available as sample schema. Select the _Samples_ tab on the _Palette_ and double-click the _ORF-Repeats_ to open the sample schema.
