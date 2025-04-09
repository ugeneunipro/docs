---
title: "How to Create and Run Workflow"
weight: 600
---


# How to Create and Run Workflow

*   Select _Tools –> Workflow Designer_ or _File->New worflow_ items in the main menu.

**Result:** The Workflow Designer window appears.

*   On the _Elements_ tab of the [_Palette_](workflow-designer-window-components.md) find the [_Read alignment_](read-alignment-element.md) element. It is located in the _Data sources_ group and drag it to the [_Scene_](workflow-designer-window-components.md).

**Result:** The element is shown on the Scene.

![](/images/1474815/1835015.png)

*   Repeat the previous step for the [_Write Alignment_](write-alignment-element.md) element from the _Data sinks_ group and for the [_Align with MUSCLE_](align-with-muscle-element.md) element from the _Multiple sequence alignment_ group.

**Result:** All three elements are on the Scene.

![](/images/1474815/1835016.png)

*   Connect the elements:

*   *   Drag an arrow from the [_output port_](workflow-elements-and-connections.md) of the _Read alignment_ element to the _Align with MUSCLE_ element.
    *   Drag an arrow from the output port of the _Align with MUSCLE_ element to the _Write alignment_ element.

**Result:** The elements are connected with arrows.

![](/images/1474815/1835017.png)

*   Select the _Read alignment_ element. In the _Parameters_ area of the [_Property Editor_](workflow-designer-window-components.md) click on the _Value_ column of the _Input files_ parameter:

![](/images/1474815/1835018.png)

*   And browse for an input file, e.g.Select the $UGENE\\data\\samples\\CLUSTALW\\COI.aln file.

**Result:** The _Input files_ value is set to the file’s path.

*   Select the _Write alignment_ element and set the _Output file_, e.g. you can just enter result.aln.

**Result:** All required workflow parameters are set.

*   Click the _Run workflow_ button on the toolbar.

![](/images/1474815/1835019.png)

**Result:** After the workflow has run, a blue notification has pop up.

*   Open the the result.aln file in UGENE.

**Result:** The file has been opened. It contains the result of the alignment with MUSCLE.
