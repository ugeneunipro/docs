---
title: "PHYLIP Neighbor-Joining"
weight: 200
---


# PHYLIP Neighbor-Joining

The _Building Phylogenetic Tree_ dialog for the _PHYLIP Neighbour-Joining_ method has the following view:


![](/images/65929715/65929716.png)

The following parameters are available:

_Distance matrix model_ — model to compute a distance matrix. The following values are available for a nucleotide multiple sequence alignment:

*   *   F84
    *   Kimura
    *   Jukes-Cantor
    *   LogDet

The following models are available for a protein alignment:

*   *   Jones-Taylor-Thornton
    *   Henikoff/Tillier PMB
    *   Dayhoff PAM
    *   Kimura

_Gamma distributed rates across sites_ — specifies to take into account unequal rates of change at different sites. It is assumed that the distribution of the rates follows the Gamma distribution.

_Coefficient of variation of substitution rate among sites_ — becomes available if the _Gamma distributed rates across sites_ parameter is checked. Specifies the coefficient of the distribution of the rates.

_Transition/transversion ratio_ — expected ratio of transitions to transversions.

To enable bootstrapping check the _Bootstrapping and Consensus Trees_ group check box. The following parameters are available:

_Number of replicates_ — number of replicate date sets.

_Seed_ — random number seed. By default, it is generated automatically. You can manually change this value in order to make results of different runs (of a tree building) reproducible. The should must be an integer greater than zero and less than 32767 and which is of the form 4n+1, that is, it leaves a remainder of 1 when divided by 4. Any odd number can also be used, but may result in a random number sequence that repeats itself after less than the full one billion numbers. Usually this is not a problem.

_Consensus type_ — specifies the method to build the consensus tree. Select one of the following:

*   *   _Strict_ — specifies that a set of species must appear in all input trees to be included in the strict consensus tree.
    *   _Majority Rule (extended)_ — specifies that any set of species that appears in more than 50% of the trees is included. The program then considers the other sets of species in order of the frequency with which they have appeared, adding to the consensus tree any which are compatible with it until the tree is fully resolved. This is the default setting.
    *   _M1_ — includes in the consensus tree any sets of species that occur among the input trees more than a specified fraction of the time (see the _Fraction_ parameter below). The _Strict_ consensus and the _Majority Rule_ consensus are extreme cases of the Ml consensus, being for fractions of 1 and 0.5 respectively.
    *   _Majority Rule_ — specifies that a set of species is included in the consensus tree if it is present in more than half of the input trees.

_Fraction_ — becomes available when the _Consensus type_ parameter is set to _M1_. Specifies the fraction.

_Display tree in new window_ - displays tree in new window.

_Display tree with alignment editor_ - displays tree with alignment editor.

_Synchronize alignment with tree_ - synchronize alignment and tree.

_Save tree to_ — file to save the tree built.

Press the _Build_ button to build a tree with the parameters selected.
