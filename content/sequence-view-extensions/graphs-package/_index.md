---
title: "Graphs Package"
weight: 400
---

# Graphs Package

The _DNA/RNA Graphs Package_ draws contextual graphs for sequences. It is available for both the Standard DNA and Standard RNA alphabets.

To use it, open a sequence in the _Sequence View_ and click on the _Graphs_ icon in the toolbar. A popup menu will appear:

![](/images/65929568/65929569.png)

To view a graph, select the corresponding item from the popup menu. A new area displaying the graph will appear directly above the _Sequence zoom view_:

![](/images/65929568/65929570.png)

Each point on the graph is calculated for a specified window size, and this window moves along the sequence by a set step. Refer to [_Graph Settings_](https://local.ugene.unipro.ru/wiki/display/UUOUM21/Graph+Settings) for instructions on modifying these parameters.

You can obtain information about each point of a graph. When you move the mouse over the _Graphs_ area, a small circle appears on the graph along with a coordinates hint above it. Holding Shift and clicking on a graph locks the circle and the hint:

![](/images/65929568/65929571.png)

To remove the hint, simply click on it. You can also delete all labels through the _Graph->Delete all labels_ context menu. To select all extremum points, use the _Graph->Select all extremum points_ context menu item.

All graphs are aligned with the range shown in the _Sequence zoom view_. This means that if you change the visible range by zooming or scrolling, the graph will update accordingly. The minimum and maximum values of the visible range are displayed at the lower and upper right corners of the graph.

To close a graph, simply uncheck its item in the popup menu.