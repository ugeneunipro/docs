---
title: "Exporting Consensus Variations"
weight: 500
---

# Exporting Consensus Variations

To export consensus sequence variations of the assembly, select the _Export Consensus Variations_ item in the _Consensus Area_ context menu.

The following dialog will appear:

![](/images/65929848/65929849.png)

Select a file, mode, and file format. The available modes are: _Variations_, _Similar_, and _All_. Variations can be exported to a SimpleSNP or VCFv4 file.

Modify the [_consensus algorithm_](../consensus-sequence) if required.

The consensus is exported with gaps if the _Keep gaps_ checkbox is checked.

You can also select the exporting region. It can be either a _Whole sequence_, a _Visible_ region, or a _Custom_ region.

When all the parameters are set, click the _Export_ button.

The consensus sequence is exported to the file, and if the _Add to project_ checkbox is checked, it is added to the current _project_ and opened.

The _Export Consensus Variations_ feature is available when the reference sequence is associated with the assembly.