---
title: "Restriction Analysis"
weight: 900
---


# Restriction Analysis

From this chapter you can learn how to search for restriction sites on a DNA sequence.

The restriction sites found are stored as automatic annotations. This means that if the automatic annotations highlighting is enabled then the restiction sites are searched and highlighted for each nucleotide sequence opened. Refer [_Automatic Annotations Highlighting_](https://local.ugene.unipro.ru/wiki/display/UUOUM22/Automatic+Annotations+Highlighting) to learn more.

Open a DNA sequence in and click the following button on the _Sequence View_ toolbar:

![](/images/65930747/96665601.png)

The _Find restriction sites_ dialog appears:

![](/images/65930747/113541195.png)

### The tree of restriction enzymes

Restriction enzymes are collected in a tree view. Enzymes are grouped by their names first letter here. Click on the **\>** icon of a group (or just double click on the entire line) to show the whole group. Check the checkbox to include enzyme to the search list and uncheck to exclude. Use **Name filter** to find certain enzyme by its name.

### Checked enzymes

Here you may see the all checked enzymes. This enzymes will be searched after clicking **OK**.

### Selected enzyme info

Some information about the enzyme selected. It includes name, link to the [REBASE](http://rebase.neb.com/rebase/rebase.html) database, the enzyme type detailed information, number of enzymes in the current sequence and sites and cuts location.

### Control buttons (right side)

*   **Open enzymes** - open file with enzymes in [the bairoch format](http://rebase.neb.com/rebase/rebase.f19.html). It is required if you want to update enzymes database or open a database with some limited amount of enzymes. See [Using Custom File with Enzymes](using-custom-file-with-enzymes) for details.
*   **Export enzymes** -  export selected enzymes to the separate file (using [the bairoch format](http://rebase.neb.com/rebase/rebase.f19.html)).
*   **Select all** - check all enzymes in the tree.
*   **Select none** - uncheck all enzymes in the tree.
*   **Select by length** - check enzymes only if its recognition site has length more than you set in the dialog window appeared.
*   **Invert selection** - switch checked and unchecked enzymes.
*   **Load selection** - load selected enzymes from the file. This file should contain comma-separated enzyme name list, for example: _BamHI,BglII,ClaI,DraI,EcoRI,EcoRV,HindIII,PstI,SalI,SmaI,XmaI_
*   **Save selection** - save checked enzymes to the separate file using the format, described above.
*   **REBASE info** - open the [REBASE](http://rebase.neb.com/rebase/rebase.html) database page of the selected enzyme.

### The filter of the results number

Show enzyme only if there are not less than "Minimum hints" and not more than "Maximum hints" values.

### Enzyme table filter

Show/hide enzymes depending on certain parameters:

*   **Suppliers** - check/uncheck suppliers, whose enzymes will be shown. By default, enzymes with undefined commercial suppliers are not shown.
*   **Recognition sequence length** - show only enzymes, whose recognition sequence length is in bounds. NOTE: **N** bases are not included in recognition site. That means, that if enzyme has the following sequence:

    C C N N N N N N N G G
    its recognition site length will be **four**, not eleven.

*   **Overhang type** - show only enzymes with certain overhang type. The following options are presented:
    *   Any - show all enzymes.
    *   No overhang - site has no cuts at all. _Example:_

        3' CTCGAG 5'
        5' GAGCTC 3'

    *   5' - the cut of the forward strand is to the **left** of the cut of the reverse-complementary strand. _Example:_

        3'  C C▼T N A G G  5'
        5'  G G A N T▲C C  3'

    *   3' - the cut of the forward strand is to the **right** of the cut of the reverse-complementary strand. _Example:_

        3'  C G A T▼C G  5'
        5'  G C▲T A G C  3'

    *   Blunt - cuts are located in the middle of the site.
    *   Sticky - cuts are locate anywhere but the middle of the site. It is 5' and 3' both.
    *   Nondegenerate sticky - the same as Sticky, but the overhang between cuts has only A, C, G or T  (no extended) symbols.
    *   Blunt or sticky - Blunt + Sticky.
    *   Blunt or nondegenerate sticky - Blunt + Nondegenerate sticky.
*   **Keep only** - show most interesting enzymes only:
    *   Palindromic - forward and reverse-complementary strands are equal.
    *   Uninterrupted - no internal **N** bases.
    *   Nondegenerate - no extended DNA alphabet symbols (only **A**, **C**, **G**, **T** and **N**).

### Search region

The region to search enzymes in. If you check the **Uncut area** checkbox,.than restriction enzymes, which exists outside of the **uncut area**, but also presisted inside of it, won't be included in the result.

Example:

You will find **two** "AsaI" enzymes in the following sequence if you choose the whole sequence as **Search in**:
![](/images/65930747/113541197.png)

But, if you also set **Uncut area** to 60-90 you will not find enzymes at all and will see the following sing in the log: The following enzymes were found, but skipped because they are presented inside of the "Uncut area": Aasi.


The information about enzymes was obtained from the [REBASE](http://rebase.neb.com/rebase/rebase.html) database. For each enzyme in the list a brief description is available (the accession ID in the database, the recognition sequence, etc.). If you’re online you can get more detailed information about an enzyme selected by clicking the _REBASE Info_ button.
