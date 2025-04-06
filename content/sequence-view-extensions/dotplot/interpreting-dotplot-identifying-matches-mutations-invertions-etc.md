---
title: "Interpreting Dotplot - Identifying Matches, Mutations, Invertions, etc"
weight: 1
---


# Interpreting Dotplot - Identifying Matches, Mutations, Invertions, etc

Using a dotplot graphic, you can identify such the following differences between the sequences:

**1\. Matches**

A _match_ between sequences looks like a diagonal line on the dotplot graphic, representing the continuous match (or repeat).

**2\. Frame shifts**

**a. Mutations**

_Mutations_ are distinctions between sequences. On the graphic they are represented by gaps in diagonal lines. They interrupt matches.

**b. Insertions**

_Insertions_ are parts of one sequence that are missed in the another, while the surrounding parts match. In other words, an insertion is a subsequence that was inserted into a sequence.

Graphically, insertions are represented by gaps which lie only on one axis. A little shift towards the other axis indicates a mutation involved.

**c. Deletions**

A deletion is a subsequence that was deleted from a sequence.

A deletion from sequence A found in sequence B can be considered as an insertion into sequence B and contained in sequence A.


![](/images/65929597/65929598.png)

**3\. Inverted repeats**

The [_Dotplot_](dotplot.md) plugin allows to search for inverted repeats as well. Inverted repeats are shown contrary to the direct repeats.

Use the _Search direct repeats_ and _Search inverted repeats_ options of the _Dotplot_ parameters dialog to select which repeats to draw (the dialog is described [_here_](http://ugene.unipro.ru/documentation/manual/sequence_view_extensions/dotplot/create_a_dotplot.html#create-a-dotplot)).


![](/images/65929597/65929599.png)

**4\. Low-complexity regions**

A low-complexity region is a region produced by redundancy in a particular part of the sequence. It is represented on a plot as a rectangular area filled with the matches.


![](/images/65929597/65929600.png)

**Hint**

Compare sequence with itself to easily find low-complexity regions in it.
