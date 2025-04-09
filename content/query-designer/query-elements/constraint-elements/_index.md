---
title: "Constraint Elements"
weight: 200
---


# Constraint Elements

To add a constraint element add the required algorithm elements to the scene and drug&drop the required constraint element.

When a _constraint element is added_, two _algorithm elements_ are selected.

There are four types of constraints that you can impose on the positional relationship of the results obtained from the algorithms calculations: _End-Start_, _Start-End_, _End-End_ and _Start-Start_.

On the image below you can see a _schema_ with [_Pattern_](../algorithm-elements/pattern-algorithm-element) and [_ORF_](../algorithm-elements/orf-algorithm-element) algorithm elements and an [_End-Start_](end-start-constraint-element) constraint:


![](/images/65930685/65930686.png)

This means the following:

1\. The algorithm elements specify to analyze the sequence with Pattern and ORF algorithms. The results of these analyses are the sets of annotations.

2\. The condition says that the distance between a “Pattern annotation end” and an “ORF annotation start” should be within the specified bounds, i.e.:

Let:

**pattern\_annot\_end** := the last nucleotide of an annotation obtained from the Pattern algorithm calculations

**orf\_annot\_start** := the first nucleotide of an annotation obtained from the ORF algorithm calculations

The constraint is:

0bp <= Distance(**pattern\_annot\_end**, **orf\_annot\_start**) <= 100bp

Find the details on each constraint element below.
