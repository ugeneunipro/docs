---
title: "Repeats Finding"
weight: 1
---


# Repeats Finding

The _Repeats Finding_ algorithm allows users to find repeated subsequences in accordance with the specified parameters.

Open a DNA sequence in the _Sequence View_. There are two ways to open the _Find Repeats_ dialog:

1.  By clicking on the toolbar button:
    ![](/images/65930735/96666087.png)
2.  By selecting the _Analyze ‣ Find repeats..._ context menu item:

![](/images/65930735/96666088.png)

The dialog following dialog appears:

### ![](/images/65930735/96666089.png)Parameters of the _Base_ page

**Repeat finder parameters**

*   _Window size_ - to put it simply, this is the minimum length of a single repeat.
*   _Minimum identity per window_ - the minimum identity of repeated subsequences (in persentage).
*   _Minimum/Maximum distance between repeats_ - it is obvious.

**Region to process**

*   _Region_ - specifies the region of the sequence that will be used to search for repeats. By default, if a subsequence has been selected when the dialog has been opened, then the selected subsequence is searched for the pattern. Otherwise, the whole sequence is used. You can also input a custom range.

**Save annotations**

*   The result annotations will be saved using [_the annotations saving_](https://doc.ugene.net/wiki/display/UM/Creating+Annotation) parameters (_Annotation name_, _Group name_, _Annotation type, Description_ and a file to save the annotation to).

### Parameters of the _Advansed_ page

![](/images/65930735/96666090.png)

_Advansed_ parameters:

*   _Custom algorithm_ - choose calculation algorithm. It will not affect results, but may affect the calculation time:
    *   _Auto_ (recommended) - the most suitable algorithm will be choosen automatically.
    *   _Suffix index_ - the search window moves along the entire sequence, each time adding one character at the end and removing one character at the beginning. The algorithm calculation time directly depends on the length of the sequence.
    *   _Diagonals_ - the [Divide-and-conquer](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm) algorithm, the subsequences are split in half recursively. More applicable for large sequences.
*   _Search only for repeats that lie inside of an annotated region._
*   _Search only for repeats that have an annotated region inside._
*   _Filter (get rid of) repeats that have an annotated region inside._
*   _Nested repeats filter algorithm_ \- how to process nested repeats:
    *   _No filtering_ \- all possible repeats will be found.
    *   _Disjoint repeats_ - repeats in which the left and right parts intersect will be filtered out.
    *   _Unique repeats_ - only pairs of repeats that occur only once in the sequence (even if repeats intersect each other).
*   _Search for inverted repeats_ - search for repeats, which are located on differend DNA strands.
*   _Exclude tandem areas_ - exclude repeats if there are three or more of them and they come in a row (use the [Tandem Repeats Finding](tandem-repeats-finding.md) feature for this case).

### Results

The found repeats are saved and displayed as annotations to the DNA sequence:

![](/images/65930735/65930737.png)
