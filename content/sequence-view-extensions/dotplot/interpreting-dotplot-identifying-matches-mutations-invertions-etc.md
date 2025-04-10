---
title: "Interpreting Dotplot - Identifying Matches, Mutations, Inversions, etc"
weight: 500
---

# Interpreting Dotplot - Identifying Matches, Mutations, Inversions, etc

Using a dotplot graphic, you can identify the following differences between the sequences:

**1\. Matches**

A _match_ between sequences appears as a diagonal line on the dotplot graphic, representing a continuous match (or repeat).

**2\. Frame shifts**

**a. Mutations**

_Mutations_ are differences between sequences. On the graphic, they are represented by gaps in diagonal lines. These gaps interrupt matches.

**b. Insertions**

_Insertions_ are parts of one sequence that are missing in another, while the surrounding parts match. In other words, an insertion is a subsequence that was inserted into a sequence.

Graphically, insertions are represented by gaps that lie only on one axis. A slight shift towards the other axis indicates a mutation is involved.

**c. Deletions**

A _deletion_ is a subsequence that has been removed from a sequence.

A deletion from sequence A, found in sequence B, can be considered an insertion into sequence B when contained in sequence A.

![Example of Dotplot](/images/65929597/65929598.png)

**3\. Inverted repeats**

The [_Dotplot_](dotplot.md) plugin also allows for the search of inverted repeats. Inverted repeats are shown as opposed to direct repeats.

Use the _Search direct repeats_ and _Search inverted repeats_ options in the _Dotplot_ parameters dialog to select which repeats to depict (the dialog is described [_here_](http://ugene.unipro.ru/documentation/manual/sequence_view_extensions/dotplot/create_a_dotplot.html#create-a-dotplot)).

![Inverted Repeats Example](/images/65929597/65929599.png)

**4\. Low-complexity regions**

A low-complexity region is characterized by redundancy in a particular part of the sequence. It is represented on a plot as a rectangular area filled with matches.

![Low-complexity Regions Example](/images/65929597/65929600.png)

**Hint**

Compare a sequence with itself to easily find low-complexity regions within it.