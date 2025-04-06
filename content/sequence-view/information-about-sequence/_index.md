---
title: "Information about Sequence"
weight: 1
---


# Information about Sequence

Statistics about an opened sequence can be found on the _Statistics_ tab of the _Options Panel_. When a region is selected in the sequence, the statistics are interactively re-calculated for this region only. The following information is available:

*   Common statistics (length, molecular weight, etc.) - see the detailed description below
*   Characters occurrence
*   Dinucleotides occurrence - available for nucleotide sequences only
*   Codons occurrence - available for nucleotide sequences only
*   Amino  acids occurrence - available for nucleotide sequences only

Note that all data, displayed on the _Statistics_ tab, can be selected with the mouse and copied. Use the copy item in the context menu or a shortcut - Ctrl+C on Windows or Linux, Cmd+C on macOS.

Nucleotide sequence common statistics
-------------------------------------

The following common statistical information is calculated for a nucleotide sequence:

*   _Length_
*   _GC content_
*   _Molecular weight_
*   _Extinction coefficient_
*   _Melting temperature_
*   _nmole/OD260_
*   _μg/OD260_

### GC content

The percentage of guanine (G) and cytosine (C) bases within the sequence or its selected region, for example:

**GC-content("ACGTAC") = ((0 + 1 + 1 + 0 + 0 + 1) / 6) \* 100% = 50%**

If the sequence contains degenerate base characters, average values are used, for example:

**GC-content("ACGNBCT") = ((0 + 1 + 1 + 1/2 + 2/3 + 1 + 0) / 7) \* 100% ~= 59.52%**

In this example "1/2" is used for "N" (any nucleotide), "2/3" us used for "B" (that means "C", "G", or "T" according to the IUPAC nucleotide code).

### Molecular weight

_Molecular weight_ for a single-stranded molecule is calculated as a sum of the atomic masses of the molecule compounds:

**DNA molecular weight  = nA\*251.24 + nT\*242.23 + nC\*227.22 + nG\*267.24 + (n-1)\*61.97**

**RNA molecular weight = nA\*267.24 + nU\*244.20 + nC\*243.22 + nG\*283.24 + (n-1)\*61.97**

Here "nA", "nT", "nC", "nG", "nU" denote the number of the corresponding nucleotide in the molecule, "n" is the number of all bases (61.97 is the weight of an internal phosphate).

Note that for degenerate base characters average value of nucleotide weight is used, for example, if the sequence also contain "Y" characters (that is "C" or "T"), the sum will include one more summand - "nY\*(242.23 + 227.22)/2".

_Molecular weight_ for a double-stranded molecule is calculated as the sum of the single strands molecular weights.

To calculate the _Extinction coefficient_, an approach proposed by Richard Owczarzy is used: [http://www.owczarzy.net/extinctionDNA.htm](http://www.owczarzy.net/extinctionDNA.htm). That is for a single-stranded molecule:

**Extinction coefficient = sum(extinction coefficients of all dinucleotides) - sum(extinction coefficients of inner mononucleotides)**

For example, let's calculate the molar extinction coefficient ("ε") for "ATGCA":

**ε(ATGCA) = ε(AT) + ε(TG) + ε(GC) + ε(CA) - ε(T) - ε(G) - ε(C) =**

                      **= 22800 + 19000 + 17600 + 21200 - 8700 - 11500 - 7400 =**

                      **= 53000**

As for the other statistics, average values are used in case of degenerate base characters.

_Extinction coef__ficient_for a double-stranded molecule is calculated as a sum of the extinction coefficients of the two single strands (es1 + es2) multiplied by coefficient of (1 - hypochromicity h260nm). The hypochromicity effect can be taken into account as follows:

**h260nm = (0.287fAT + 0.059fGC)**

where _f_AT and _f_GC are fractions of AT and GC base pairs, respectively.

### Melting temperature

Click on the gear icon ![](/images/65929387/94078798.png)near Melting temperature label and the Melting temperature settings dialog will be opened.
Note, that  UGENE computes Tm fot sequence regions from 8 to 10000 bp. Otherwise, an undefined value N/A is output.

See [the corresponding page](https://doc.ugene.net/wiki/display/UM/Melting+tempeature) for settings details.

### nmole/OD260

The amount of DNA or RNA represented in nanomoles per 1 unit of absorbance at 260 nm dissolved in 1 ml cuvette with 1 cm pathlength.

**nmole/OD260 = 1000000 / molarExtCoef**

### μg/OD260

The amount of DNA or RNA represented in microgrames per 1 unit of absorbance at 260 nm dissolved in 1 ml cuvette with 1 cm pathlength.

**μg/OD260 = nmoleOD260 \* molarWeight \* 0.001**

Amino acid sequence common statistics
-------------------------------------

The following common statistical information is calculated for an amino acid sequence:

*   _Length_
*   _Molecular weight_
*   _Isoelectic point_
