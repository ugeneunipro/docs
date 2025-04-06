---
title: "Locking and Synchronize Ranges of Several Sequences"
weight: 1
---


# Locking and Synchronize Ranges of Several Sequences

An important feature of the _Sequence zoom view_ is the ability to synchronize and lock visual ranges of different sequences shown in the _Sequence View_.

This feature is available when there are two or more sequences opened in the same _Sequence View_.

If we click the _Lock scales_ button the second sequence scale will be adjusted to be the same as the focused sequence scale and is locked. Now if we move a scrollbar or use zoom buttons for any of the sequence, visual ranges for the rest sequences will also be adjusted.


![](/images/65929447/65929448.png)

To unlock the scales click the same button again.

You may use the _Adjust scales_ button to synchronize scales without locking them.

Note, that if you have a selected sequence region or a selected annotation the scales will be synchronized by the start position of the region or the annotation. If there are no active selection the regions are synchronized by the first visible sequence position on the screen.
