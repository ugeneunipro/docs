---
title: "Melting tempeature"
weight: 1
---


# Melting tempeature

There are two algorithms for melting temperature calculation:

*   Rough
*   Primer 3

Note, that Rough works only for DNA alphabet, it does not work for DNA extended and RNA alphabets. Primer3 works for all extended alphabets.

Rough
-----

The melting temperature is calculated as follows. For sequences of length 15 or longer:

**Tm \= **64.9 + 41 \* (nG + nC - 16.4) / (nA + nT + nG + nC)****

For shorter sequences:

**Tm \= (nA + nT) \* 2 + (nG + nC) \* 4**

Here "nA", "nT", "nC", "nG" denote the number of the corresponding nucleotide.

Primer 3
--------

This calculation algorithm is borrowed from [the Primer3 package](https://github.com/primer3-org/primer3). The algorithm uses the nearest-neighbor (NN) model or the formula from Bolton and McCarthy, PNAS 84:1390 (1962) (as presented in Sambrook, Fritsch and Maniatis, Molecular Cloning, p 11.46 (1989, CSHL Press)). The algorithm has the following parameters:

*   _DNA concentration_ (nanomolar) - a value to use as nanomolar concentration of each annealing oligo over the course the PCR. This parameter corresponds to 'c' in equation (ii) of the paper \[SantaLucia (1998) A unified view of polymer, dumbbell, and oligonucleotide DNA nearest-neighbor thermodynamics. Proc Natl Acad Sci 95:1460-1465 [http://www.pnas.org/content/95/4/1460.full.pdf+html](http://www.pnas.org/content/95/4/1460.full.pdf+html)\], where a suitable value (for a lower initial concentration of template) is "empirically determined".
*   _Monovalent concentration_ (millimolar) - the millimolar concentration of monovalent salt cations (usually KCl) in the PCR.
*   _Divalent concentration_ (millimolar) - the millimolar concentration of divalent salt cations (usually MgCl^(2+)) in the PCR.
*   _DNTP concentration_ (millimolar) - the millimolar concentration of the sum of all deoxyribonucleotide triphosphates. A reaction mix containing 0.2 mM ATP, 0.2 mM CTP, 0.2 mM GTP and 0.2 mM TTP would have this value equals to 0.8.
*   _DMSO concentration_ (%) - the concentration of DMSO in percent.
*   _DMSO factor_ \- The melting temperature of primers can be approximately corrected for DMSO:

    **Tm \= Tm**(without DMSO) + DMSO factor \* DMSO concentration****

*   _Formamide concentration_ (mol/l) - The concentration of formamide in mol/l. The melting temperature of primers can be approximately corrected for formamide:

    **Tm \= Tm**(without formamide) + (0.453 \* GC% / 100 - 2.88)  \* Formamide concentration****

*   _NN Max Length_ - the maximum sequence length for using the nearest neighbor model. For sequences longer than this, algorithm uses the "GC%" formula from Bolton and McCarthy, PNAS 84:1390 (1962):

    **Tm \= 81.5 - DMSO concentration \* DMSO factor** **+ 0.453 \* (**GC%** \- 2.88) \* Formamide concentration + 16.6 \* log10(Monovalent concentration / 1000) + 0.41 \* **GC%** \- 600 / **Length****

*   _Thermodynamic table_ - specifies the thermodynamic table for the melting temperature calculation:
    *   Breslauer - method for Tm calculations from the paper \[Rychlik W, Spencer WJ and Rhoads RE (1990) "Optimization of the annealing temperature for DNA amplification in vitro", Nucleic Acids Res 18:6409-12 [https://academic.oup.com/nar/article/18/21/6409/2388653?login=false](https://academic.oup.com/nar/article/18/21/6409/2388653?login=false)\] and the thermodynamic parameters from the paper\[Breslauer KJ, Frank R, Blocker H and Marky LA(1986) "Predicting DNA duplex stability from the base sequence" Proc Natl Acad Sci 83:4746-50 [http://dx.doi.org/10.1073/pnas.83.11.3746](http://dx.doi.org/10.1073/pnas.83.11.3746)\]
    *   SantaLucia \- method for Tm calculations and the thermodynamic parameters from \[SantaLucia JR (1998) "A unified view of polymer, dumbbell and oligonucleotide DNA nearest-neighbor thermodynamics", Proc Natl Acad Sci 95:1460-65 [http://dx.doi.org/10.1073/pnas.95.4.1460](http://dx.doi.org/10.1073/pnas.95.4.1460)\]
*   _Salt Correction Formula_ - specifies the salt correction formula for the melting temperature calculation:
    *   Schildkraut - \[Schildkraut, C, and Lifson, S(1965) "Dependence of the melting temperature of DNA on salt concentration", Biopolymers 3:195-208 (not available on-line)\]
    *   SantaLucia - \[SantaLucia JR(1998) "A unified view of polymer, dumbbell and oligonucleotide DNA nearest - neighbor thermodynamics", Proc Natl Acad Sci 95:1460-65 [http://dx.doi.org/10.1073/pnas.95.4.1460](http://dx.doi.org/10.1073/pnas.95.4.1460)\]
    *   Owczarzy - \[Owczarzy, R., Moreira, B.G., You, Y., Behlke, M.A., and Walder, J.A. (2008) "Predicting stability of DNA duplexes in solutions containing magnesium and monovalent cations", Biochemistry 47 : 5336 - 53 [http://dx.doi.org/10.1021/bi702363u](http://dx.doi.org/10.1021/bi702363u)\]
