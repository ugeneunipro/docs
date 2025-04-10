---
title: "Plasmid Auto Annotation"
weight: 200
---

# Plasmid Auto Annotation

The Plasmid Auto Annotation feature allows you to automatically annotate possible functional elements of a given sequence, such as promoters, terminators, origins of replication, known genes, common primers, and other features. Conceptually, this functionality is similar to that offered by the [PlasMapper](https://plasmapper.wishartlab.com/) software. The database for plasmid auto-annotation is based on the following [resource.](http://www.addgene.org/tools/reference/plasmid-features/)

To activate Plasmid Auto Annotation on your sequence, use the menu item _Analyze ‣ Annotate plasmid._ In the dialog that appears, you can select the features to search in the sequence.

![](/images/65930930/65930932.png)

The detected plasmid features are stored as automatic annotations and can be controlled through the corresponding menu. Refer to [_Automatic Annotations Highlighting_](../../sequence-view/annotations-editor/automatic-annotations-highlighting) to learn more.

Plasmid Auto Annotations consist of 471 carefully selected and annotated plasmid features broken down into 12 feature categories. These are shown in the following table:

| Type of Feature                                                                                                                                     | Number of Features |
|-----------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| [Promoter](https://en.wikipedia.org/wiki/Promoter_\(genetics\))                                                                                     | 50                 |
| [Terminator](https://en.wikipedia.org/wiki/Terminator_\(genetics\))                                                                                 | 29                 |
| [Regulatory sequence](https://en.wikipedia.org/wiki/Regulatory_sequence)                                                                            | 65                 |
| [Replication origin](https://en.wikipedia.org/wiki/Origin_of_replication)                                                                           | 12                 |
| [Selectable marker](https://en.wikipedia.org/wiki/Selectable_marker)                                                                                | 26                 |
| [Reporter gene](https://en.wikipedia.org/wiki/Reporter_gene)                                                                                        | 40                 |
| [Two-hybrid gene](https://en.wikipedia.org/wiki/Two-hybrid_screening)                                                                               | 12                 |
| [Localization sequence](https://en.wikipedia.org/wiki/Nuclear_localization_sequence)                                                                | 15                 |
| [Affinity tag](https://en.wikipedia.org/wiki/Protein_tag)                                                                                           | 21                 |
| [Gene](https://en.wikipedia.org/wiki/Gene)                                                                                                          | 7                  |
| [Primer](https://en.wikipedia.org/wiki/Primer_\(molecular_biology\))                                                                                | 77                 |
| Miscellaneous                                                                                                                                       | 117                |
| **Total**                                                                                                                                           | **471**            |

This feature database has been created by combining the original FASTA formatted PlasMapper 2.0 feature database (which had 336 features) with [AddGene’s sequence feature database](https://www.addgene.org/), followed by extensive manual editing, duplicate removal, validation, and cleaning.