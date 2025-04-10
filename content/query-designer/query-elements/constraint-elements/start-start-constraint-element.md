---
title: "Start-Start Constraint Element"
weight: 400
---

# Start-Start Constraint Element

[_Add the Start-Start constraint_](../../manipulating-query-designer-element/adding-constraint-element) to two _algorithm elements_. Let's denote these elements as **alg1** and **alg2**.

Parameters in GUI
-----------------

| Parameter       | Description                                                                         | Default Value |
|-----------------|-------------------------------------------------------------------------------------|---------------|
| **Min distance** | Minimum distance between an **alg1** annotation start and an **alg2** annotation start. | 0bp           |
| **Max distance** | Maximum distance between an **alg1** annotation start and an **alg2** annotation start. | 0bp           |

**Constraint Explanation:**

Let:

- **alg1_annot_start** := the first nucleotide of an annotation obtained from **alg1**.
- **alg2_annot_start** := the first nucleotide of an annotation obtained from **alg2**.

The resulting annotations should comply with the rule:

**Min distance** <= Distance(**alg1_annot_start**, **alg2_annot_start**) <= **Max distance**

Parameters in Schema File
-------------------------

**Type:** distance

**Distance-type:** start-to-start

| Parameter | Parameter in the GUI | Type     |
|-----------|----------------------|----------|
| **min**   | **Min distance**     | _numeric_ |
| **max**   | **Max distance**     | _numeric_ |