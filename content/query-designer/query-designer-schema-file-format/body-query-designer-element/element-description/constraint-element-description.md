---
title: "Constraint Element Description"
weight: 200
---

# Constraint Element Description

When describing a constraint element, the **element\_name** consists of two parts separated by two hyphens:

part1--part2

Each part represents one of the algorithms the constraint is imposed on.

If the algorithm is presented as a single element in a schema (like [_ORF_](../../../query-elements/algorithm-elements/orf-algorithm-element) or [_Pattern_](../../../query-elements/algorithm-elements/pattern-algorithm-element)), the algorithm’s part has the format:

algorithm\_element\_name.unit

If the algorithm is presented as two subelements in a schema (like [_Repeats_](../../../query-elements/algorithm-elements/repeats-algorithm-element) or [_Primer_](../../../query-elements/algorithm-elements/primer-algorithm-element)), the algorithm’s part has the format:

algorithm\_element\_name.left

or:

algorithm\_element\_name.right

depending on the subelement the constraint is imposed on.

You should also specify the constraint type parameter (currently, the only available type is _distance_):

type: distance;

And specify one of the distance types, for example:

distance-type: end-to-start;

**Example 1:** The constraint is imposed on **myORF** and **myPattern** algorithm elements:

myORF.unit--myPattern.unit {

   type: distance;
   distance-type: start-to-start;

   # Other parameters
}

**Example 2:** The constraint is imposed on the **myORF** algorithm element and the left **myRepeats** algorithm subelement:

myORF.unit--myRepeats.left {

   type: distance;
   distance-type: start-to-end;

   # Other parameters
}

The available constraint elements are described in the [_Constraint Elements_](constraint-elements.md) chapter.