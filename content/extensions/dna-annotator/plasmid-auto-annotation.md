---
title: "Plasmid Auto Annotation"
weight: 1
---


# Plasmid Auto Annotation

Plasmid Auto Annotation feature allows to automatically annotate possible functional elements of the given sequence such as promoters, terminators, origin of replication, known genes, common primers and other features. Conceptually this functionality is similar to the one offered by [PlasMapper](https://plasmapper.wishartlab.com/) software. The database for plasmid auto-annotation is based on the following [resource.](http://www.addgene.org/tools/reference/plasmid-features/)

To activate Plasmid Auto Annotation upon your sequence use the menu item _Analyze ‣ Annotate plasmid._ In the appeared dialog one can selected the features to search in sequence.

![](/images/65930930/65930932.png)

The detected plasmid features are stored as automatic annotations and can be controlled through corresponding menu. Refer [_Automatic Annotations Highlighting_](automatic-annotations-highlighting.md) to learn more.

Plasmid Auto Annotations consists 471 carefully selected and annotated plasmid features broken down into 12 feature categories. These are shown in the followind table:

Type of feature

Number of features

[Promoter](https://en.wikipedia.org/wiki/Promoter_\(genetics\))

50

[Terminator](https://en.wikipedia.org/wiki/Terminator_\(genetics\))

29

[Regulatory sequence](https://en.wikipedia.org/wiki/Regulatory_sequence)

65

[Replication origin](https://en.wikipedia.org/wiki/Origin_of_replication)

12

[Selectable marker](https://en.wikipedia.org/wiki/Selectable_marker)

26

[Reporter gene](https://en.wikipedia.org/wiki/Reporter_gene)

40

[Two-hybrid gene](https://en.wikipedia.org/wiki/Two-hybrid_screening)

12

[Localization sequence](https://en.wikipedia.org/wiki/Nuclear_localization_sequence)

15

[Affinity tag](https://en.wikipedia.org/wiki/Protein_tag)

21

[Gene](https://en.wikipedia.org/wiki/Gene)

7

[Primer](https://en.wikipedia.org/wiki/Primer_\(molecular_biology\))

77

Miscellaneous

117

**Total**

471

This features database has been created by combining the original FASTA formatted PlasMapper 2.0 feature database (which had 336 features) with [AddGene’s sequence feature database](https://www.addgene.org/) followed by extensive manual editing, duplicate removal, validating and cleaning.
