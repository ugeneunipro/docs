---
title: "Primer-BLAST"
weight: 100
---

# Primer-BLAST

You can run BLAST for primer pairs similar to [this tool](https://www.ncbi.nlm.nih.gov/tools/primer-blast/). This tool allows you to screen primers against a user-selected database to avoid primer pairs that can cause non-specific amplifications. Your primers should be in Primer3 UGENE format. You can obtain them using [Primer3](primer3.md)/[Primer3 (no target sequence)](/docs/extensions/primer3/primer3-no-target-sequence) or by using the special [Transform into a primer pair](../../sequence-view/annotations-editor/transform-into-a-primer-pair) feature.

Select the primer pairs you need to BLAST:

![](/images/96666281/96666286.png)

Right-click and select Analyze → Query NCBI BLAST database...:

![](/images/96666281/96666287.png)

The following dialog has exactly the same settings as the regular [Remote BLAST](remote-blast.md) tool, except:

* Instead of "Save annotation(s) to" and "Annotations parameters," you will see a list of selected primer pairs. This means that BLAST will be run three times for three primer pairs - **pair 1**, **pair 4**, and **pair 3**. All results will be stored in the annotation group associated with the primer pair that was input for this calculation.
* The "Megablast" option is enabled by default. Disable this option to get more results (note that it affects calculation time).