---
title: "End-End Constraint Element"
weight: 300
---


# End-End Constraint Element

[_Add the End-End constraint_](../../manipulating-query-designer-element/adding-constraint-element) to some two _algorithm elements_. Lets denote these elements as **alg1** and **alg2**.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Min distance**

Minimum distance between an **alg1** annotation end and an **alg2** annotation end.

0bp

**Max distance**

Maximum distance between an **alg1** annotation end and an **alg2** annotation end.

0bp

**Constraint Explanation:**

Let:

**alg1\_annot\_end** := the last nucleotide of an annotation obtained from the **alg1**.

**alg2\_annot\_end** := the last nucleotide of an annotation obtained from the **alg2**.

The result annotations should comply with the rule:

**Min distance** <= Distance(**alg1\_annot\_end**, **alg2\_annot\_end**) <= **Max distance**

Parameters in Schema File
-------------------------

**Type:** distance

**Distance-type:** end-to-end

Parameter

Parameter in the GUI

Type

**min**

**Min distance**

_numeric_

**max**

**Max distance**

_numeric_
