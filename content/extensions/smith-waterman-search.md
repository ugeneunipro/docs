---
title: "Smith-Waterman Search"
weight: 1500
---

# Smith-Waterman Search

The _Smith-Waterman Search_ plugin adds a complete implementation of [the Smith-Waterman algorithm](https://en.wikipedia.org/wiki/Smith%E2%80%93Waterman_algorithm) to UGENE.

To use the plugin, open a nucleotide or protein sequence in the _Sequence View_ and select the _Analyze ‣ Find pattern \[Smith-Waterman\]_ item in the context menu. The _Smith-Waterman Search_ dialog appears:

![](/images/65930804/65930807.png)

### Algorithm

This search algorithm has a significant advantage in calculation time over the usual _[Search in sequence](https://doc.ugene.net/wiki/pages/viewpage.action?pageId=65929429&from=ugene)_ algorithm for large sequences. This happens because the "_Search in sequence_" algorithm represents a suffix algorithm - one sequence moves along the other, and areas opposite each other are compared. Using this approach, the computation time increases in direct proportion to the length of the sequence. The _Smith-Waterman algorithm_ uses a completely different approach - searching using a certain kind of matrix.

The algorithm works in the following way:

1. A matrix is created where the sequence in which the search is carried out is located vertically, and the searched sequence is located horizontally. Fill the adjacent row and column with 0. Example:
   The sequence in which the search is carried out - ACGCGAT.
   The searched sequence - CGCG.

   ```
   D(i,j)

     C   G   C   G
   0 0   0   0   0
   A 0
   C 0
   G 0
   C 0
   G 0
   A 0
   T 0
   ```

2. Start filling the matrix from the top-left corner, moving from left to right and from top to bottom, using the following formula:
   ![](/images/65930804/96666056.png)
   Where:
   _D(S1, S2)_ - current cell,
   _D(S1-1, S2)_ - the cell on the left,
   _D(S1, S2-1)_ - the cell above,
   _D(S1-1, S2-1)_ - the one on the top and left,
   _gap_ - the _Gap open_ penalty if we encounter a gap for the first time and the _Gap extension_ penalty if we encounter a gap the second time or more.
   _score_ - the value from the _Scoring matrix_ table.
   The following example uses **nucl** _Scoring matrix_ (**+5** for match, **-4** for mismatch) and **-1** for _Gap open_ and _Gap extension_ penalties:

   ![](/images/65930804/96666057.png)

3. Find the largest number and move to the top, left, or top-left to the next larger number:
   ![](/images/65930804/96666058.png)
   Matching green symbols indicate the desired sequence intersection.

### Parameters

First of all, you need to specify the pattern to search for. The rest of the parameters are optional:

_Search in_ — select either to search in the sequence or in its amino acid translation.

_Strand_ — select the strand to search in: direct, reverse-complementary, or both strands.

_Region_ — specifies the region of the sequence that will be used to search for the pattern. By default, if a subsequence has been selected when the dialog has been opened, then the selected subsequence is searched for the pattern. Otherwise, the whole sequence is used. You can also input a custom range.

_Algorithm version_ — version of the algorithm implementation. All versions produce the same result - only the inner technology is used differently:

- _Classic 2_ - classical implementation of the algorithm. Works everywhere.
- _SSE2_ - the algorithm, which works much faster, but requires you to have an [SSE2](https://en.wikipedia.org/wiki/SSE2) processor.

_Scoring matrix_ — can be chosen from a variety of matrices supplied with UGENE. To view a selected matrix, click the _View_ button.

_Gap open_ — penalty for opening a gap.

_Gap extension_ — penalty for extending a gap.

_Report results_ — simple heuristic which allows filtering of intersected hits. If it is set to _none_, the algorithm may report a large set of almost identical results in the same region.

_Minimal score_ — another simple heuristic which measures sequence similarity. It is more convenient than using some abstract scores. If set to 100%, the algorithm will search for an exact substring match.

### Input and output

The results of the search are saved as annotations or as multiple alignments. To set the saving parameters, go to the _Input and output_ tab of the dialog.

- If you want to save the results as annotations, input [_the annotations saving_](../sequence-view/manipulating-annotations/creating-annotation) parameters (_Annotation name_, _Group name_, _Annotation type_, _Description_ and a file to save the annotation to). You can also add a qualifier with corresponding pattern subsequences to result annotations. Check the corresponding checkbox for this.
- If you want to save the results as multiple alignments, select the following parameters:

  ![](/images/65930804/96666059.png)

  Here you can select a file to save the alignment to (_Alignment files directory path_ parameter).

Using the _Set advanced options_ checkbox, you can select the saving options.

You can set different templates for file names: create your own or create using the following: \[E\] — adds a subsequence end position, \[hms\] — adds a time, \[MDY\] — adds a date, \[S\] — adds a subsequence start position, \[L\] — adds a subsequence length, \[SN\] — adds a reference sequence name prefix, \[PN\] — adds a pattern sequence name prefix, \[C\] — adds a counter.

You can create templates for alignment file names, reference subsequence names, pattern subsequence names, and for the pattern sequence name:

![](/images/65930804/65930805.png)