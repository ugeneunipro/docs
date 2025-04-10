---
title: "Spliced Alignment mRNA and cDNA"
weight: 3200
---

# Spliced Alignment mRNA and cDNA

UGENE allows you to align spliced mRNA/cDNA sequences to genomic sequences.

The default algorithm used for this alignment is an external tool called [Spidey](http://www.ncbi.nlm.nih.gov/spidey/).

Before running the alignment, ensure that Spidey is available and validated in the list of _[External Tools](#)_.

To perform the alignment of an mRNA sequence to a genomic sequence, open the genomic sequence in the _Sequence View_. Next, activate the context menu item _Align -> Align to sequence to mRNA_.

![](/images/65930923/65930924.png)

In the list of sequences, select the corresponding mRNA sequence and click OK.

The following dialog will appear:

![](/images/65930923/65930925.png)

Here, you can set up a file to store annotations. It could be either an existing annotation table object, a new annotation table, or an auto-annotations table (if applicable). Also, you can modify the group name parameter and add a description.

The resulting alignment will be saved as an annotation with the corresponding name:

![](/images/65930923/65930926.png)