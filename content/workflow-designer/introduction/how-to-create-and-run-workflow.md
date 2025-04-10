---
title: "How to Create and Run Workflow"
weight: 600
---

# How to Create and Run Workflow

1. Select _Tools –> Workflow Designer_ or _File -> New workflow_ from the main menu.

   **Result:** The Workflow Designer window appears.

2. On the _Elements_ tab of the [_Palette_](workflow-designer-window-components), find the [_Read alignment_](../workflow-elements/data-readers/read-alignment-element) element. It is located in the _Data sources_ group. Drag it to the [_Scene_](workflow-designer-window-components).

   **Result:** The element is displayed on the Scene.

   ![](/images/1474815/1835015.png)

3. Repeat the previous step for the [_Write Alignment_](../workflow-elements/data-writers/write-alignment-element) element from the _Data sinks_ group and the [_Align with MUSCLE_](../workflow-elements/multiple-sequence-alignment/align-with-muscle-element) element from the _Multiple sequence alignment_ group.

   **Result:** All three elements are on the Scene.

   ![](/images/1474815/1835016.png)

4. Connect the elements:

   - Drag an arrow from the [_output port_](workflow-elements-and-connections) of the _Read alignment_ element to the _Align with MUSCLE_ element.
   - Drag an arrow from the output port of the _Align with MUSCLE_ element to the _Write alignment_ element.

   **Result:** The elements are connected by arrows.

   ![](/images/1474815/1835017.png)

5. Select the _Read alignment_ element. In the _Parameters_ area of the [_Property Editor_](workflow-designer-window-components), click on the _Value_ column of the _Input files_ parameter:

   ![](/images/1474815/1835018.png)

6. Browse for an input file, for example, select the $UGENE\\data\\samples\\CLUSTALW\\COI.aln file.

   **Result:** The _Input files_ value is set to the file’s path.

7. Select the _Write alignment_ element and set the _Output file_, for example, you can just enter result.aln.

   **Result:** All required workflow parameters are set.

8. Click the _Run workflow_ button on the toolbar.

   ![](/images/1474815/1835019.png)

   **Result:** After the workflow has run, a blue notification pops up.

9. Open the result.aln file in UGENE.

   **Result:** The file is opened and contains the result of the alignment with MUSCLE.