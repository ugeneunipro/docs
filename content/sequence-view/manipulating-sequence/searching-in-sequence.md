---
title: "Searching in Sequence"
weight: 1000
---


# Searching in Sequence

To search for a pattern(s) in a sequence go to the _Search in Sequence_ tab of the _Options Panel_ in the _Sequence View_.

Input the value you want to search in the text field. To search multiple patterns input the patterns separated by a new line in the pattern text field. To add a new line symbol _Ctrl+Enter_ may be used. You can input the value as a sequence or name of the sequence in the FASTA format and sequence after that. Press the _Next_ button to search in the direction “From left to right”. Press the _Previous_ button to search in the direction “From right to left”. If the pattern is found, the result will be focused and highlighted in the _Sequence area_. You can continue the search in any direction from this position.


![](/images/65929429/65929430.png)

By default, **misc\_feature** annotations are created for regions that exactly match the pattern. Find below the description of the available settings.

### Load Patterns from File


![](/images/65929429/65929431.png)

Use this option to load patterns from a file. When this option is active the _Search for_ field is disabled.

### Search Algorithm


![](/images/65929429/65929432.png)

This group specifies the algorithm that should be used to search for a pattern. The algorithm can be one of the following:

*   _InsDel_ — there could be insertions and/or deletions, i.e. a pattern and the searched region can vary in their length. You can specify the percentage of the pattern and a searched region match in the field nearby. Note that this value also depends on the pattern length and is disabled when the pattern hasn’t been specified.
*   _Substitute_ — a pattern may contain characters different from the characters in the searched region. When this algorithm has been selected you can also specify the match percentage and additionally it is possible to take into account ambiguous bases.
*   _Regular expression_ — a regular expression may be specified instead of a pattern. For example character ‘.’ matches any character, ‘.\*’ matches zero or more of any characters. There is also the _Result no longer than_ option that specifies the maximum length of a result.


    ![](/images/65929429/65929433.png)

*   _Exact_ - find a place where one or several patterns are found within a larger pattern.

### Search in


![](/images/65929429/65929434.png)

In this group you can specify where to search for a pattern: in what region and in which strand (for nucleotide sequences). Also for nucleotide sequences, it is possible to search for a pattern on the sequence translations.

_Strand_ — for nucleotide sequences only. Specifies on which strand to search for a pattern: _Direct_, _Reverse-complementary_ or _Both_ strands.

_Search in_ — for nucleotide sequences you can select the _Translation_ value for this option. In this case, the input pattern will be searched in the amino acid translations.

_Region_ — specifies the sequence range where to search for a pattern. You can search in the whole sequence, specify a custom region or search in the selected region.

### Other Settings


![](/images/65929429/65929435.png)

This group contains additional common settings:

_Remove overlapped results_ — annotates only one of the overlapped results.

_Limit results number to_ — limits the number of the searched results to the specified value.

### Annotations Settings


![](/images/65929429/65929436.png)

In the _Save annotation(s) to_ group, you can set up a file to store annotations.  It could be either an existing annotation table object or a new annotation table.

In the _Annotation parameters_ group, you can specify the name of the group and the name of the annotation. If the group name is set to <auto> UGENE will use the group name as the name for the group. You can use the ‘/’ characters in this field as a group name separator to create subgroups. If the annotation name is set to _by type_ UGENE will use the annotation type from the _Annotation type:_ table as the name for the annotation. Also you can add a description in the corresponding text field. To use a pattern name for the annotations check the corresponding checkbox.

After that click the _Create annotations_ button. The annotations will be created.

### _Searching for one or several patterns and names of the result annotations_

If you search for one pattern only, then input the required name into the _Annotation name_ field and leave the _Use pattern name_ checkbox unchecked.

You can also search for several patterns at a time by:

*   Inputting several patterns into the search field (click _<Ctrl> + <Enter>_ keys to insert to a new line):
    ![](/images/65929429/65929436.png)




*   Inputting several patterns into the search filed in FASTA format:
    ![](/images/65929429/65929437.png)
*   Loading patterns from a FASTA file

Even when you search for several patterns, the names of the found annotations will be identical by default (the name is specified in the _Annotation name_ field).

If you want to assign different names to annotations found for different patterns, then you should:

*   Input the patterns in FASTA format (the latter two cases above)
*   Check the _Use pattern name_ checkbox in the _Annotation parameters_ group

Here is an example of the found annotations in the [Annotations Editor](annotations-editor.md):

![](/images/65929429/65929438.png)



---
