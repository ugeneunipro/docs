---
title: "Primer-BLAST"
weight: 1
---


# Primer-BLAST

You can run BLAST for primer pairs as in [the corresponding tool](https://www.ncbi.nlm.nih.gov/tools/primer-blast/). This tool allows one to screen primers against user-selected database in order to avoid primer pairs that can cause non-specific amplifications. You primers should have Primer3 UGENE format. Either get them using [Primer3](primer3.md)/[Primer3 (no target sequence)](96666247.html) or create by using the special [Transform into a primer pair](transform-into-a-primer-pair.md) feature.

Select primer pairs you need to BLAST:

![](/images/96666281/96666286.png)

Click right mouse button → Analyze → Query NCBI BLAST database...:

![](/images/96666281/96666287.png)

The foolowing dialog has absolutely the same settings as the regular [Remote BLAST](remote-blast.md) tool, except:

*   Instead of "Save annotation(s) to" and "Annotations paramters" settings you can see a list of selected primer pairs. That means, that BLAST will be run three times for three primer pairs - **pair 1**, **pair 4** and **pair 3**. All results will be stored to the annotation group with a primer pair, which was an input for this calculation.
*   The "Megablast" option is enabled by default. Disable this option to get more results (it affects calculation time).
