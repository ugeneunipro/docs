---
title: "ORF Marker"
weight: 500
---

# ORF Marker

In this chapter, you can learn how to search for Open Reading Frames (ORF) within a DNA sequence. The ORFs identified are stored as automatic annotations. This means that if the automatic annotations highlighting has been enabled, ORFs are searched for and highlighted in each sequence opened. Refer to [_Automatic Annotations Highlighting_](../sequence-view/annotations-editor/automatic-annotations-highlighting) to learn more.

To open the _ORF Marker_ dialog, select the _Analyze ‣ Find ORFs_ item in the context menu.

![](/images/65930706/65930707.png)

The following **Search Settings** are available:

- **_Min length_** — ORFs with lengths shorter than the _Min length_ value will not be found.
- **_Must terminate within region_** — this option ignores boundary ORFs located beyond the search region.
- **_Must start with init codon_** — this item switches the ORF Marker algorithm to the mode where any non-stop amino acid code is interpreted as the region start position.
- **_Allow overlaps_** — alternative (downstream) initiators, when another start codon is located within a longer ORF, i.e., all possible ORFs will be found, not only the longest ones.
- **_Allow alternative init codon_** — this option includes ORFs starting with alternative initiation codons, according to the current translation table.
- **_Include stop codon_** — this option includes stop codons in the resulting annotations.
- **_Max result_** — this option allows you to define the maximum number of results to be found.

The other available parameters are:

- **DNA-to-Amino translation table** defines how start, alternative start, and stop codons are encoded.
- **Strand** — specifies where to search for the ORFs: in the direct strand, in the complement strand, or in both strands.
- **Preview** — allows you to preview the regions, strands, and lengths of the found ORFs.
- **Clear results** — becomes available when some results have been found; this clears those results.

To set the saving parameters, go to the _Output_ tab of the dialog.

Here you can modify [_the annotations saving_](https://ugene.unipro.ru/wiki/display/UUOUM17/Creating+Annotation) parameters (_Group name_, _Description_, and a file to save the annotation to).

Results:

When the search parameters have been selected and the _OK_ button has been pressed in the dialog, the _auto-annotating_ feature becomes enabled. In the _Annotations editor_, the ORFs annotations can be found in the Auto-annotations\\orf group.

After the search has been completed, you can browse the results, sort them by length, strand, or start position, and save them as annotations to the original sequence in the Genbank format.

For more information about codons, use the codon table. To show or hide the table, use the _Ctrl+T_ shortcut or click the _Show codon table_ toolbar button menu.

![](/images/65930706/65930708.png)

The codon table will appear:

![](/images/65930706/65930709.png)

Clicking on a codon name redirects you to Wikipedia, providing a brief description of the corresponding amino acid. The cells of the table are colored according to the classes of amino acids.