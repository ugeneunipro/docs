---
title: "Find Group of Annotated Regions"
weight: 100
---


# Find Group of Annotated Regions

The _Find Group of Annotated Regions_ feature provides an algorithm to search for sequence regions that contain a predefined set of annotations.

Open a DNA sequence in the _Sequence View_. There are two ways to open the _Find Repeats_ dialog:

1.  By clicking on the toolbar button:
    ![](/images/65930692/96666131.png)

2.  By selecting the _Analyze ‣ Find annotated regions..._ context menu item:

### ![](/images/65930692/96666132.png)

### Algorithm

This tool has been designed to search for annotations that intersect (or completely overlap - it depends on the specified parameters) other, already existing annotations of a given sequence. Let's look at the example:![](/images/65930692/96666133.jpg)

We have a sequence with two annotations. Annotations have different lengths and do not intersect each other. The _annotation 2_ length is **four** times the _annotation 1_ length (41 vs. 11 bases).

Using this function, we can find an annotation that intersects both source annotations and captures their shares depending on their lengths. For example, lets find an intersection 25 bases long. We will have the following annotation:

![](/images/65930692/96666134.jpg)

As we can see, the intersection with the first annotation is **two** characters long, and the intersection with the second annotation is **eight** characters long. This result was chosen because the second annotation is **four** times the length of the first annotation.

![](/images/65930692/96666135.jpg)

**NOTE**: A good candidate for this feature could be any file in Genbank format with a rich set of annotations. FASTA is not the best option, because this format does not store annotations.

### Parameters



![](/images/65930692/96666136.png)The following parameters are avaliable:

*   _Left window_ - annotations to search intersection regions for.
*   _Right window_ - the list of possible intersection regions.
*   _Region size_ - the length of the new intersection region.
*   _Result strand_ - select the DNA strand whose annotations will be considered in the search. If, for example, the "Complement" strand is selected, but all choosen annotations are on the direct strand, than nothing will be found.
*   _Annotation must fit into region_ - all annotations, choosen at the _left window_, must fit completely to the result annotation (completely - not just in a few characters).
*   _Save regions as annotations_ \- store results to annotations.
*   _Clear results_ - clear the result table.
