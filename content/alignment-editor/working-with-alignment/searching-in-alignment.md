---
title: "Searching in Alignment"
weight: 400
---


# Searching in Alignment

To search for a pattern(s) in an alignment, navigate to the _Search in Alignment_ tab within the _Options Panel_.

![](/images/65929651/65929652.png)

The following parameters are available:

### Search Context

This group specifies the search context to be used for searching a pattern. It is possible to search for patterns in sequences or sequence names.

### Search Pattern

To search for a pattern(s), input the value you want to search in the text field.

Press the _Next_ button to search in the direction “From left to right, from top to bottom.” Press the _Previous_ button to search in the direction “From right to left, from bottom to top.” If the pattern is found, the result will be focused on and highlighted in the _Sequence area_. You can continue the search in any direction from this position.

To group results, press the _Group_ button. The results will be selected and grouped at the top after the first click or at the bottom after the second click of the button.

### Search Algorithm

This group specifies the algorithm to be used to search for a pattern. The algorithm can be one of the following:

- _InsDel_ — There could be insertions and/or deletions, i.e., a pattern and the searched region can vary in their length. You can specify the percentage of the pattern and a searched region match in the field nearby. Note that this value also depends on the pattern length and is disabled when the pattern hasn’t been specified.
- _Substitute_ — A pattern may contain characters different from the characters in the searched region. When this algorithm has been selected, you can also specify the match percentage, and additionally, it is possible to take into account ambiguous bases.
- _Regular Expression_ — A regular expression may be specified instead of a pattern. For example, the character ‘.’ matches any character, ‘.*’ matches zero or more of any characters. There is also the _Limit result length_ option that specifies the maximum length of a result.
- _Exact_ — Find a place where one or several patterns are found within a larger pattern.

### Search In

In this group, you can specify the sequence range where to search for a pattern. You can search in the whole alignment, specify a custom region, or search in the selected region.

### Other Settings

This group contains additional common settings:

_Remove overlapped results_ — Annotates only one of the overlapped results.

_Limit results number to_ — Limits the number of the searched results to the specified value.