---
title: "Start-End Constraint Element"
weight: 200
---


# Start-End Constraint Element

_[Add the Start-End constraint](adding-constraint-element.md)_ to some two _algorithm elements_. Lets denote these elements as **alg1** and **alg2**.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Min distance**

Minimum distance between an **alg1** annotation start and an **alg2** annotation end.

0bp

**Max distance**

Maximum distance between an **alg1** annotation start and an **alg2** annotation end.

0bp

**Constraint Explanation:**

Let:

**alg1\_annot\_start** := the first nucleotide of an annotation obtained from the **alg1**.

**alg2\_annot\_end** := the last nucleotide of an annotation obtained from the **alg2**.

The result annotations should comply with the rule:

**Min distance** <= Distance(**alg1\_annot\_start**, **alg2\_annot\_end**) <= **Max distance**

Parameters in Schema File
-------------------------

**Type:** distance

**Distance-type:** start-to-end

Parameter

Parameter in the GUI

Type

**min**

**Min distance**

[_numeric_](http://ugene.unipro.ru/documentation/qd_manual/qd_schema_file_format/body/elt_description.html#term-query-numeric-parr)

**max**

**Max distance**

[_numeric_](http://ugene.unipro.ru/documentation/qd_manual/qd_schema_file_format/body/elt_description.html#term-query-numeric-parr)
