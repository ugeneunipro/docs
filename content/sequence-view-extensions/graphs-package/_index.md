---
title: "Graphs Package"
weight: 1
---


# Graphs Package

The _DNA/RNA Graphs Package_ draws contextual graphs for sequences. The _DNA/RNA Graphs Package_ is available for the Standard DNA and Standard RNA alphabets.

Open a sequence in the _Sequence View_ and click the _Graphs_ icon on the toolbar. The popup menu appears:


![](/images/65929568/65929569.png)

To see a graph select the corresponding graph item in the popup menu. A new area with the graph appears right above the _Sequence zoom view_:


![](/images/65929568/65929570.png)

Each point on a graph is calculated for a window of a specified size. The window is moved along the sequence by a step. See [_Graph Settings_](https://local.ugene.unipro.ru/wiki/display/UUOUM21/Graph+Settings) for instructions on how to modify these parameters.

It is possible to get information about each point of a graph. When a mouse is moved in the _Graphs_ area, a small circle shows on the graph. A coordinates hint shows above it. When you hold Shift and click on a graph, the circle and the hint locks:


![](/images/65929568/65929571.png)

To remove it click on the hint. Also, you can delete all labels by _Graph->Delete all labels_ context menu. To select all extremum points use the _Graph->Select all extremum points_ context menu item.

All graphs are always aligned with the range shown in the _Sequence zoom view_. It means that if you change the visible range in the overview (either by zooming or scrolling) the graph will also be updated. The minimum and maximum values of the visible range are shown at the right lower and upper corners of the graph.

To close a graph, uncheck its item in the popup menu.

*   [Description of Graphs](description-of-graphs.md)
*   [Graph Settings](graph-settings.md)
*   [Saving Graph Cuttoffs as Annotations](saving-graph-cuttoffs-as-annotations.md)


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
