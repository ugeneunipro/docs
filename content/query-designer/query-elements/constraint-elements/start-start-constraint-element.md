---
title: "Start-Start Constraint Element"
weight: 400
---


# Start-Start Constraint Element

[_Add the Start-Start constraint_](adding-constraint-element.md) to some two _algorithm elements_. Lets denote these elements as **alg1** and **alg2**.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Min distance**

Minimum distance between an **alg1** annotation start and an **alg2** annotation start.

0bp

**Max distance**

Maximum distance between an **alg1** annotation start and an **alg2** annotation start.

0bp

**Constraint Explanation:**

Let:

**alg1\_annot\_start** := the first nucleotide of an annotation obtained from the **alg1**.

**alg2\_annot\_start** := the first nucleotide of an annotation obtained from the **alg2**.

The result annotations should comply with the rule:

**Min distance** <= Distance(**alg1\_annot\_start**, **alg2\_annot\_start**) <= **Max distance**

Parameters in Schema File
-------------------------

**Type:** distance

**Distance-type:** start-to-start

Parameter

Parameter in the GUI

Type

**min**

**Min distance**

_numeric_

**max**

**Max distance**

_numeric_
