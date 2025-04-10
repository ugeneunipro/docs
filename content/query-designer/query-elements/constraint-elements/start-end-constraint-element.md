---
title: "Start-End Constraint Element"
weight: 200
---

# Start-End Constraint Element

[Add the Start-End constraint](../../manipulating-query-designer-element/adding-constraint-element) to two algorithm elements. Let's denote these elements as **alg1** and **alg2**.

Parameters in GUI
-----------------

| Parameter      | Description                                                   | Default value |
|----------------|---------------------------------------------------------------|---------------|
| **Min distance** | Minimum distance between an **alg1** annotation start and an **alg2** annotation end. | 0bp           |
| **Max distance** | Maximum distance between an **alg1** annotation start and an **alg2** annotation end. | 0bp           |

**Constraint Explanation:**

Let:

- **alg1_annot_start** be the first nucleotide of an annotation obtained from **alg1**.
- **alg2_annot_end** be the last nucleotide of an annotation obtained from **alg2**.

The result annotations should comply with the rule:

**Min distance** <= Distance(**alg1_annot_start**, **alg2_annot_end**) <= **Max distance**

Parameters in Schema File
-------------------------

| Type            | Description            |
|-----------------|------------------------|
| **Type:**       | distance               |
| **Distance-type:** | start-to-end        |

| Parameter | Parameter in the GUI | Type |
|-----------|----------------------|------|
| **min**   | **Min distance**     | [_numeric_](http://ugene.unipro.ru/documentation/qd_manual/qd_schema_file_format/body/elt_description.html#term-query-numeric-parr) |
| **max**   | **Max distance**     | [_numeric_](http://ugene.unipro.ru/documentation/qd_manual/qd_schema_file_format/body/elt_description.html#term-query-numeric-parr) |