---
title: "Searching in Alignment"
weight: 1
---


# Searching in Alignment

To search for a pattern(s) in alignment go to the _Search in Alignment_ tab of the _Options Panel_.


![](/images/65929651/65929652.png)

The following parameters are available:

### Search context

This group specifies the search context that should be used to search for a pattern. It is possible to search patterns in sequences or in sequence names.

### Search pattern

To search for a pattern(s) input the value you want to search in the text field.

Press the _Next_ button to search in the direction “From left to right, from top to bottom”. Press the _Previous_ button to search in the direction “From right to left, from bottom to top”. If the pattern is found, the result will be focused and highlighted in the _Sequence area_. You can continue the search in any direction from this position.

To group results press _Group_ button. The results will be selected and grouped to the top after the first click or to the bottom after the second click to the button.

### Search Algorithm

This group specifies the algorithm that should be used to search for a pattern. The algorithm can be one of the following:

*   _InsDel_ — there could be insertions and/or deletions, i.e. a pattern and the searched region can vary in their length. You can specify the percentage of the pattern and a searched region match in the field nearby. Note that this value also depends on the pattern length and is disabled when the pattern hasn’t been specified.
*   _Substitute_ — a pattern may contain characters different from the characters in the searched region. When this algorithm has been selected you can also specify the match percentage and additionally it is possible to take into account ambiguous bases.
*   _Regular expression_ — a regular expression may be specified instead of a pattern. For example character ‘.’ matches any character, ‘.\*’ matches zero or more of any characters. There is also the _Limit result length_ option that specifies the maximum length of a result.
*   _Exact_ \- find a place where one or several patterns are found within a larger pattern.

### Search in

In this group, you can specify the sequence range where to search for a pattern. You can search in the whole alignment, specify a custom region or search in the selected region.

### Other Settings

This group contains additional common settings:

_Remove overlapped results_ — annotates only one of the overlapped results.

_Limit results number to_ — limits the number of the searched results to the specified value.
