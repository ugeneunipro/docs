---
title: "Constraint Element Description"
weight: 1
---


# Constraint Element Description

When you describe a constraint element the **element\_name** consists of two parts separated by two hyphens.

part1--part2

Each part represents one of the algorithms the constraint is imposed on.

If the algorithm is presented as one element on a schema (like [_ORF_](orf-algorithm-element.md), [_Pattern_](pattern-algorithm-element.md)) the algorithm’s part has format:

algorithm\_element\_name.unit

If the algorithm is presented as two subelements on a schema (like [_Repeats_](repeats-algorithm-element.md), [_Primer_](primer-algorithm-element.md)) the algorithm’s part has format:

algorithm\_element\_name.left

or:

algorithm\_element\_name.right

depending on the subelement the constraint is imposed on.

Also you should specify the constraint type parameter (currently the only available type is _distance_):

type: distance;

And specify one of the distance types, for example:

distance-type: end-to-start;

**Example1:** The constraint is imposed on **myORF** and **myPattern** algorithm elements:

myORF.unit--myPattern.unit {

   type: distance;
   distance-type: start-to-start;

   # Other parameters
}

**Example2:** The constraint is imposed on **myORF** algorithm element and the left **myRepeats** algorithm subelement:

myORF.unit--myRepeats.left {

   type: distance;
   distance-type: start-to-end;

   # Other parameters
}

The available constraint elements are described in the [_Constraint Elements_](constraint-elements.md) chapter.
