---
title: "Description of Graphs"
weight: 100
---

# Description of Graphs

Below is a detailed description of each graph. Note that the characters A, C, G, and T in the formulas represent the number of corresponding nucleotides in a window.

*   _DNA Flexibility_ — Identifies regions of high DNA helix flexibility in a DNA sequence. The average _Threshold_ in a window is calculated using the following formula:

    \[
    \frac{\text{sum of flexibility angles in the window}}{\text{window size} - 1}
    \]

    For more detailed information, see the [_DNA Flexibility_](https://ugene.unipro.ru/wiki/display/UUOUM/DNA+Flexibility) section.

*   _GC Content (%)_ — Shows the percentage of nitrogenous bases (either guanine or cytosine) in a DNA molecule. It is calculated using the formula:

    \[
    \frac{(G+C)}{(A+G+C+T)} \times 100
    \]

*   _AG Content (%)_ — Shows the percentage of nitrogenous bases (either adenine or guanine) in a DNA molecule. It is calculated using the formula:

    \[
    \frac{(A+G)}{(A+G+C+T)} \times 100
    \]

*   _GC Frame Plot_ — This graph is similar to the GC content graph but shows the GC content of the first, second, and third positions independently. It is most effective in organisms with GC-rich genomic sequences but also works on all microbial sequences.

*   _GC Deviation (G-C)/(G+C)_ — Shows the difference between the “G” content of the forward strand and that of the reverse strand. _GC Deviation_ is calculated using the formula:

    \[
    \frac{(G-C)}{(G+C)}
    \]

*   _AT Deviation (A-T)/(A+T)_ — Shows the difference between the “A” content of the forward strand and that of the reverse strand. _AT Deviation_ is calculated using the formula:

    \[
    \frac{(A-T)}{(A+T)}
    \]

*   _Karlin Signature Difference_ — Represents the dinucleotide absolute relative abundance difference between the whole sequence and a sliding window. Let:

    \[
    f(XY) = \text{frequency of the dinucleotide XY}
    \]
    \[
    f(X)  = \text{frequency of the nucleotide X}
    \]

    \[
    p(XY) = \frac{f(XY)}{f(X) \times f(Y)}
    \]

    \[
    p\_seq(XY) = p(XY) \text{ for the whole sequence}
    \]
    \[
    p\_win(XY) = p(XY) \text{ for a window}
    \]

    The _Karlin Signature Difference_ for a window is calculated using the formula:

    \[
    \frac{\sum(p\_seq(XY) - p\_win(XY))}{16}
    \]

*   _Informational Entropy_ — Calculated from a table of overlapping DNA triplet frequencies. The use of overlapping triplets smooths the frame effect. _Informational Entropy_ is calculated using the formula:

    \[
    \-(\text{triplet frequency}) \times \log_{10}(\text{triplet frequency})/\log_{10}(2)
    \]