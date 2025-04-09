---
title: "DNA Flexibility"
weight: 200
---


# DNA Flexibility

To search for regions of high DNA helix flexibility in a DNA sequence, open the sequence in the _Sequence View_ and select the _Analyze ‣ Find high DNA flexibility regions_ item in the context menu. Note that only standard DNA alphabet is supported, i.e. the sequence should consist of characters A, C, G, T and N.

The following dialog appears:


![](/images/65930694/65930695.png)

The calculation is made for overlapping windows along a given sequence. If there are two or more consecutive windows with an average flexibility threshold (in each window) greater than the specified _Threshold_ parameter, such area is marked by an [_annotation_](annotations-editor.md).

The average threshold in a window is calculated by the following formula:

(average window threshold) = (sum of flexibility angles in the window) / (the window size - 1)

The following flexibility angles are used during the calculation:

Dinucleotide

Angle

Dinucleotide

Angle

**AA**

7.6

**CA**

14.6

**AC**

10.9

**CC**

7.2

**AG**

8.8

**CG**

11.1

**AT**

12.5

**CT**

8.8

**GA**

8.2

**TA**

25

**GC**

8.9

**TC**

8.2

**GG**

7.2

**TG**

14.6

**GT**

10.9

**TT**

7.6

A minimum value is used when N characters is present in a dinucleotide:

*   **CN**, **NC**, **GN**, **NG**, **NN**: 7.2
*   **AN**, **NA**, **TN**, **NT** : 7.6
