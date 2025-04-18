---
title: "Coloring Schemes"
weight: 400
---

# Coloring Schemes

It is possible to apply different coloring schemes for an alignment so that nucleotide or amino acid residues are colored depending on some rules.

To set another coloring scheme, select the required item in the main menu (_Actions → Appearance → Colors_) or context menu (Appearance → _Colors_) of the _Alignment Editor_, or in the _Color_ combo box on the _Highlighting_ tab on the _Options Panel_.

![](/images/65929620/65929621.png)

Note that the coloring schemes setting may interfere with other alignment highlighting settings (see, for example, the _Highlighting_ combo box on the _Highlighting_ tab of the _Options Panel_). Thus, the colors may vary in this case from those described below.

### Coloring Schemes for Nucleotides

The following scheme options are available for nucleotide alignment:

*   _No colors_ — Do not color the residues' background (i.e., all residues have a white background and black font).
*   _Jalview_ — Use the following background colors: A - green, C - orange, G - red, T/U - blue. Gaps and characters of the extended nucleotide alphabet are not colored.
*   _Percentage identity_ — A residue's background color depends on its presence in the column of the alignment: <=40% - white, 41-60% - light slate blue, 61-80% - medium slate blue, 81-100% - dark slate blue.
*   _Percentage identity (colored)_ — Colors depend on the residues' percentage presence in a column. The following rules are applied (in the order of priority):
    *   If all residues (100%) are the same and there are no gaps, the residues in the column have a yellow background and red font.
    *   If there are 50% of one residue in the column and 50% of another (gaps are not taken into account), one-half of the residues has a green background and black font (the half to be colored is determined based on the following priorities: T>U>G>C>A>B>D>H>K>M>R>S>V>W>Y>N).
    *   If there is one or several residues in a column with a percentage number equal to or greater than the threshold parameter (see the _Threshold_ parameter on the _Highlighting_ tab of the _Options Panel_), then the most frequent residues are colored as follows: light blue background color and blue font. Note that gaps are taken into account when calculating the percentage number in the column in this case. Also, if required, the same residues' priorities are applied as in the previous rule.
    *   If the rules above are not applied for a residue, then it remains uncolored, i.e., white background color and black font are used.
*   _Percentage identity (gray)_ — This coloring scheme is similar to the _Percentage identity_ scheme, but shades of gray are used instead of slate blue.
*   _UGENE_ — This is the default coloring scheme; the following background colors are used: A - yellow, C - light green, G - light blue, T/U - light red, gap - white. Other colors may be used for characters of the extended nucleotide alphabet.
*   _UGENE Sanger_ — This coloring scheme is used in the _UGENE Sanger Reads Editor_; the background colors correspond to the peaks of Sanger chromatogram peaks: A - green, C - blue, G - light gray, T - red. The orange background color is used for a gap, and the magenta background color is used for characters of the extended nucleotide alphabet.
*   _Weak Similarities_ — When there is a choice between two characters and it is not specified by other rules which character to color, the following priorities apply: T>U>G>C>A>B>D>H>K>M>R>S>V>W>Y>N.

    Coloring rules:

    *   Do not color gaps (“-”), i.e., use a black font and white background.
    *   Residues should be colored according to their percentage number in the column (use the priorities described above in case of equal percentage numbers).
    *   Residues with the most frequency/priority in the column.
*   A [custom scheme](https://local.ugene.unipro.ru/wiki/display/UUOUM32/Creating+Custom+Color+Scheme) can be created and used with colors that depend on a residue.

### Coloring Schemes for Amino Acids

The following scheme options are available for amino acid alignment:

*   _No colors_ — Do not color the residues' background (i.e., all residues have a white background and black font).
*   _Buried index_ — Depending on the frequency of occurrence inside a globule, the amino acid residues are colored from light green (less frequent) to blue (most frequent).
*   _Clustal X_ — An emulation of the default color scheme in Clustal X, a graphical interface for the ClustalW multiple alignment programs.
*   _Helix propensity_ — Depending on helix propensity, the residues are colored from magenta (the highest helix propensity) to green (the lowest one).
*   _Hydrophobicity_ — Residues are colored based on their hydrophobicity. The most hydrophobic residues are red, and the most hydrophilic are blue.
*   _Percentage identity_ — A residue's background color depends on its presence in the column of the alignment: <=40% - white, 41-60% - light slate blue, 61-80% - medium slate blue, 81-100% - dark slate blue.
*   _Percentage identity (gray)_ — This coloring scheme is similar to the _Percentage identity_ scheme, but shades of gray are used instead of slate blue.
*   _Strand propensity_ — Residues with the highest strand propensity are yellow, while those with the lowest are blue.
*   _Tailor_ — See [this publication](https://www.ncbi.nlm.nih.gov/pubmed/9342138) by William R.Taylor.
*   _Turn propensity_ — Residues with the highest turn propensity are red, while those with the lowest are cyan.
*   _UGENE_ — This is the default coloring scheme; the following background colors are used for the residues: positive (KRH) - yellow, aromatic (FWY) - green, large aliphatic hydrophobic (ILM) - blue, small hydrophobic (ST) - rose, GP - red, EX - gray.
*   _Zappo_ — Amino acids residues are colored according to their physicochemical properties: aliphatic/hydrophobic (residues ILVAM) - rose, aromatic (FWY) - orange, positive (KRH) - dark blue, negative (DE) - red, hydrophilic (STNQ) - light green, conformationally special (PG) - magenta, cysteine (C) - yellow.
*   A [custom scheme](https://local.ugene.unipro.ru/wiki/display/UUOUM32/Creating+Custom+Color+Scheme) can be created and used with colors that depend on a character.