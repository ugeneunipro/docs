---
title: "Description of Graphs"
weight: 1
---


# Description of Graphs

Find below the detailed description of each graph. Note that characters A, C, G and T in the formulas denote the number of corresponding nucleotide in a window.

*   _DNA Flexibility_ — searches for regions of high DNA helix flexibility in a DNA sequence. The average _Threshold_ in a window is calculated by the following formula:

    (sum of flexibility angles in the window) / (the window size - 1)

    For more detailed information see [_DNA Flexibility_](https://ugene.unipro.ru/wiki/display/UUOUM/DNA+Flexibility) paragraph.

*   _GC Content (%)_ — shows the percentage of nitrogenous bases (either guanine or cytosine) on a DNA molecule. It is calculated by the following formula:

    (G+C)/(A+G+C+T)\*100

*   _AG Content (%)_ — shows the percentage of nitrogenous bases (either adenine or guanine) on a DNA molecule. It is calculated by the following formula:

    (A+G)/(A+G+C+T)\*100

*   _GC Frame Plot_ — this graph is similar to the GC content graph but shows the GC content of the first, second and third position independently. It is most effective in organisms with GC rich genomic sequence but it also works on all microbial sequences.
*   _GC Deviation (G-C)/(G+C)_ — shows the difference between the “G” content of the forward strand and the reverse strand. _GC Deviation_ is calculated by the following formula:

    (G-C)/(G+C)

*   _AT Deviation (A-T)/(A+T)_ — shows the difference between the “A” content of the forward strand and the reverse strand. _AT Deviation_ is calculated by the following formula:

    (A-T)/(A+T)

*   _Karlin Signature Difference_ — dinucleotide absolute relative abundance difference between the whole sequence and a sliding window. Let:

    f(XY) = frequency of the dinucleotide XY
    f(X)  = frequency of the nucleotide X

    p(XY) = f(XY) / f(X) \* f(Y)

    p\_seq(XY) = p(XY) for the whole sequence
    p\_win(XY) = p(XY) for a window

    The _Karlin Signature Difference_ for a window is calculated by the following formula:

    sum(p\_seq(XY) - p\_win(XY)) / 16

*   _Informational Entropy_ — is calculated from a table of overlapping DNA triplet frequencies. The use of overlapping triplets smooths the frame effect. _Informational Entropy_ is calculated by the following formula:

    \-(triplet frequency)\*log10(triplet frequency)/log10(2)
