---
title: "Aligning Sequences to Profile with MUSCLE"
weight: 300
---

# Aligning Sequences to Profile with MUSCLE

Another feature provided by the plugin is the ability to align a set of unaligned sequences to an existing profile. To use this feature, select the _Align ‣ Align sequences to profile with MUSCLE_ context menu item.

This option is not available in the original MUSCLE package (v3.7) and is a new functionality for original MUSCLE users. In this mode, each sequence from the input file is aligned to the active profile separately and is merged into the resulting alignment only after all sequences are processed. For example, the alignment in the picture above can be used as a profile again, and the added profile can be used as a set of sequences. The result of such sequences-to-profile alignment is presented in the picture below:

![](/images/65930839/65930840.png)

The original alignment is not modified; only columns with the gap ('—') character can be inserted.

The second profile was considered as a set of sequences and therefore is modified.

Note that if a file with another alignment is used as a source of unaligned sequences, the gap characters are removed and each input sequence is processed independently.

This method is quite fast; for example, an alignment of 3000 sequences (1000 bases each) to the existing profile takes about 5 minutes on a typical Core 2 Duo computer.