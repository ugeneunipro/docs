---
title: "Translating Nucleotide Sequence"
weight: 300
---

# Translating Nucleotide Sequence

When a nucleotide sequence is opened in the _Sequence View_, both the sequence and its complementary sequence are displayed by default in the _Details View_.

### Showing/Hiding the Amino Acid Sequences

It is possible to translate them and also show the corresponding amino acid sequences:

![](/images/65929396/65929397.png)

The translation settings are available on the left toolbar of the _Details View_:

![](/images/65929396/65929398.png)

The _Show/Hide Amino Acid Translations_ menu allows you to set up the mode for amino acid sequence visualization:

![](/images/65929396/65929399.png)

The following options are available:

*   _Do not translate_ — hide the amino acid sequences.
*   _Translate selection_ — translate only a selected region of the sequence and the complementary sequence.

![](/images/65929396/65929400.png)

*   _Set up frames manually_ — select the [reading frames](https://en.wikipedia.org/wiki/Reading_frame) to display. There are three frames for the sequence ("+1", "+2", "+3") and three for the complementary sequence ("-1", "-2", "-3"). Note that the complementary frame items are hidden in the menu if the complementary sequence is hidden.

![](/images/65929396/65929401.png)

*   _Show all frames_ — show all amino acid sequences.

### Setting the Genetic Code

The default value for the [genetic code](https://www.ncbi.nlm.nih.gov/Taxonomy/Utils/wprintgc.cgi) for nucleotide sequence translation is read by UGENE from the sequence file when it is available. You can also set up the genetic code for the sequence using the _Select Genetic Code_ menu:

![](/images/65929396/65929402.png)

All analysis routines (such as HMMER, ORF finding, etc.) will use this code by default.

### Codon Table

To refresh your knowledge about the amino acid codes, select the _Show Codon Table_ button ![](/images/65929396/65929397.png) on the _Sequence View_ global toolbar. The codon table appears at the upper part of the window:

![](/images/65929396/65929403.png)