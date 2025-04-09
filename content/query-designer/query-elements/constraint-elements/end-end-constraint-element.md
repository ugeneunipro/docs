---
title: "End-End Constraint Element"
weight: 300
---

# End-End Constraint Element

[Add the End-End constraint](../../manipulating-query-designer-element/adding-constraint-element) to two _algorithm
elements_. Let's denote these elements as **alg1** and **alg2**.

---

## Constraint Explanation

Let:

- **alg1_annot_end** := the last nucleotide of an annotation obtained from **alg1**
- **alg2_annot_end** := the last nucleotide of an annotation obtained from **alg2**

The result annotations must satisfy the following rule:

**Min distance** ≤ Distance(**alg1_annot_end**, **alg2_annot_end**) ≤ **Max distance**

---

## Parameters in GUI

| **Parameter** | **Description**                                                                     | **Default Value** |
|---------------|-------------------------------------------------------------------------------------|-------------------|
| Min distance  | Minimum distance between an **alg1** annotation end and an **alg2** annotation end. | 0bp               |
| Max distance  | Maximum distance between an **alg1** annotation end and an **alg2** annotation end. | 0bp               |

---

## Parameters in Schema File

| **Parameter**   | **Parameter in GUI** | **Type**     |
|-----------------|----------------------|--------------|
| `min`           | Min distance         | _numeric_    |
| `max`           | Max distance         | _numeric_    |
| `type`          | *(not in GUI)*       | `distance`   |
| `distance-type` | *(not in GUI)*       | `end-to-end` |
