---
title: "Circular Viewer"
weight: 100
---


# Circular Viewer

The _Circular Viewer_ plugin provides the capability to display a circular view of a nucleotide sequence.

**Usage example:**

Open a nucleotide sequence object in the _Sequence View_. The _Show circular view_ button is available on the sequence toolbar:

![](/images/65929513/96665864.png)

Pressing the button will display the circular view of the sequence:

![](/images/65929513/65929514.png)

If you work with a file containing many sequences, the button will close circular views if some are open, and if all are closed, it will open all of them.

Additionally, you can mark sequences as circular in UGENE through the _Mark as circular_ option in the sequence context menu. When sequences are marked as _Circular_, the Circular View will automatically open for them in all opened Sequence View windows.

The _Restriction Sites Map_ will appear automatically. To display restriction sites, the _Show Restriction Sites_ menu should be checked. To hide the map, click on the following button:

![](/images/65929513/65929515.png)

The _Circular Viewer_ opens automatically when the _Sequence View_ is opened for a plasmid.

The inner circle represents the sequence in a clockwise manner, and the scale marks show the corresponding sequence positions. The sequence annotations are represented as curved colored regions on the outer side of the circle.

The _Circular Viewer_ aids in navigating within the sequence. You can select an annotation on the circular view, and the annotation will also be focused and highlighted in all _Sequence View_ areas: _Sequence overview_, _Sequence zoom view_, _Sequence details view_, and _Annotations editor_.

You can also select a sequence region:

![](/images/65929513/65929516.png)

This selection will also affect the _Sequence View_. You can select a sequence region with _Ctrl_, and the selection will be inverted.

Note that the circular view is automatically zoomed when the _Circular Viewer_ area is resized:

![](/images/65929513/65929517.png)

You can adjust it to an appropriate size.

It is possible to rotate the circular view using the mouse wheel. Additionally, you can shift the start point of a circular molecule by using the _Edit sequence -> Set new sequence origin_ context menu item.

Use the _Export ‣ Save circular view as image_ context menu or the _Actions_ main menu item to save the circular view image:

![](/images/65929513/65929518.png)

The _Export Image_ dialog will appear:

![](/images/65929513/65929519.png)

You can set _Include position marker_ and _Include selection_ marker in the image using the corresponding checkboxes.

Here you can browse for the file name and select the width, height, and resolution of the image, as well as its format: SVG, BMP, JPG, PNG, PDF, PS, and TIFF. Pay attention to the _Quality_ slider, which is available for the JPG format only.

Note that if a sequence file contains several sequences, it is possible to view the circular views of these sequences in the same _Circular Viewer_ area:

![](/images/65929513/65929520.png)

You can work with these circular views simultaneously.