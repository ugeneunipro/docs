---
title: "Using Objects and Object Views"
weight: 1100
---

# Using Objects and Object Views

The document always contains one or more _objects_. An _object_ is structured biological data that can be visualized by different _Object Views_.

A single _Object View_ can visualize one or several objects of different types. For example, a single view can show a sequence, annotations for the sequence, a 3D model for a part of the sequence, or its chromatogram simultaneously.

The type of an object is indicated by the symbol in square brackets and the icon near the object:

![](/images/65929301/96665792.png)

Below is a list of object types supported by the current version of UGENE.

**Object Types:**

| **Symbol** | **Icon** | **Description** |
|------------|----------|-----------------|
| **\[3d\]** | ![](/images/65929301/107020514.png) | A 3D model. |
| **\[a\]**  | ![](/images/65929301/107020523.png) | Annotations for DNA sequence regions. |
| **\[as\]** | ![](/images/65929301/107020523.png) | An assembly. |
| **\[c\]**  | ![](/images/65929301/107020523.png) | Chromatogram data. |
| **\[m\]**  | ![](/images/65929301/107020511.png) | A multiple sequence alignment. |
| **\[s\]**  | ![](/images/65929301/107020519.png) | A nucleic, protein, or raw sequence. |
| **\[t\]**  | ![](/images/65929301/107020509.png) | Plain text. |
| **\[tr\]** | ![](/images/65929301/107020505.png) | A phylogenetic tree. |

You can edit the names of particular objects, such as sequence objects, by selecting them in the _Project View_ and then pressing F2. To be able to do so, the document containing the target object must be unlocked.

To see the list of all available views for a given object, select the object and activate the context menu inside the _Project View_ window, then select the _Open In_ submenu:

![](/images/65929301/107020530.png)

The picture above illustrates an option to visualize the selected DNA sequence object using the _Sequence View_ — a complex and extensible _Object View_ that focuses on the visualization of sequence objects in combination with different kinds of related data: sequence annotations, graphs, chromatograms, and sequence analysis algorithms. Note that the _Sequence View_ is described in more detail in the separate [_documentation section_](sequence-view.md).