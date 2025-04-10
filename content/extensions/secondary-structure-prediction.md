---
title: "Secondary Structure Prediction"
weight: 1300
---

# Secondary Structure Prediction

The _Secondary Structure Prediction_ plugin provides a set of algorithms for predicting protein secondary structure (alpha-helix, beta-sheet) from a raw sequence.

Currently, the available algorithms are:

* **GORIV**: Jean Garnier, Jean-Francois Gibrat, and Barry Robson, "GOR Method for Predicting Protein Secondary Structure from Amino Acid Sequence", in Methods in Enzymology, vol. 266, pp. 540 - 553, (1996).

    The improved version of the GOR method in J. Garnier, D. Osguthorpe, and B. Robson, J. Mol. Biol., vol. 120, p. 97 (1978).

* **PsiPred**: Bryson K, McGuffin LJ, Marsden RL, Ward JJ, Sodhi JS, & Jones DT. (2005) Protein structure prediction servers at University College London. Nucl. Acids Res. 33(Web Server issue): W36-38.

    Jones DT. (1999) Protein secondary structure prediction based on position-specific scoring matrices. J. Mol. Biol. 292: 195-202.

You can access these analysis capabilities for a protein sequence using the _Analyze ‣ Predict secondary structure..._ context menu item. The dialog will appear:

![](/images/65930792/65930794.bmp)

It supports the following options:

_Algorithm_ — you can choose the preferred algorithm. Currently, the “GORIV” and “PsiPred” algorithms are available.

_Region_ — select the sequence range for prediction. The region can be either a _Selected region_ if selected before prediction, _Whole sequence_ or _Custom_ region.

_Results_ — the visual representation of the prediction results, for example:

![](/images/65930792/96665942.png)

_Save_ — select this button to save the results as annotations of the current protein sequence.

![](/images/65930792/96665946.png)

Visual representation of the predicted annotation on the sequence:

![](/images/65930792/65930793.png)