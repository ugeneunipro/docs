---
title: "Selecting Sequence Region"
weight: 700
---

# Selecting Sequence Region

### Selection in the Sequence View Components

By holding down the left mouse button and moving the mouse, you can select a sequence region in the _Zoom View_ or _Details View_ components of the _Sequence View_. A sequence region that corresponds to an annotation can also be selected by [double-clicking on the annotation](../manipulating-annotations/selecting-annotations) in the _Zoom View_, _Details View_, or _Annotations Editor_.

The selection of a sequence region is synchronized among different _Sequence View_ components.

In the _Sequence Overview_, the selection is displayed as a blue line:

![](/images/65929414/65929415.png)

In the _Zoom View_, a blue line with coordinates and the length of the selected region is shown:

![](/images/65929414/65929416.png)

In the _Details View_, a rectangle with a dashed border is shown around the selected region:

![](/images/65929414/65929417.png)

### Selecting a Region Using the Mouse

You can select a region of a sequence using the mouse in each component of the _Sequence View_.

In the _Zoom View_ and the _Details View_, the selection can be adjusted by dragging its left or right border:

![](/images/65929414/65929418.png)

### Selecting a Region Using the Dialog

If you have the exact coordinates of a region, click the _Select sequence region_ button ![](/images/65929414/65929419.png) on the toolbar, or choose _Select–>Sequence region_ in the context menu of the _Sequence View_. Input the coordinates in the _Region Selection_ dialog:

![](/images/65929414/65929419.png)

You can input:

*   _Single Range Selection_ — a common region with a single range. Use the _Min_ and _Max_ buttons to automatically specify the beginning and the end of the sequence in the corresponding fields.
*   _Multiple Range Selection_ — a region that consists of several joined elements, for example, exons of a gene. See "[The DDBJ/ENA/GenBank Feature Table Definition](http://www.insdc.org/files/feature_table.html)" for details.

### Selecting a Region Around or Between Annotations

To select a region between two annotations, such as an intron region between two exons:

*   Click on the annotations while holding the _Ctrl_/_Cmd_ key:

![](/images/65929414/65929420.png)

*   Click _Select–>Sequence between selected annotations_ in the context menu of the _Sequence View_.

To select a region that contains the annotations in a single range, choose the _Sequence around selected annotations_ item in the menu.