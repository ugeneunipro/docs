---
title: "Dump Sequence Info"
weight: 300
---

# Dump Sequence Info

This workflow outputs the sequence name and sequence size for all incoming sequences.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

---

### Workflow Sample Location

The workflow sample **"Dump Sequence Info"** is located in the **"Custom Elements"** section of the Workflow Designer samples.

---

### Workflow Image

Here is what the workflow looks like:

![Workflow image](/images/65930268/65930269.png)

---

### Workflow Wizard

The wizard consists of 2 pages.

#### 1. Input sequence(s)

On this page, input your sequence(s).

![Input sequences](/images/65930268/65930270.png)

#### 2. Output data

On this page, modify output settings as needed.

![Output data](/images/65930268/65930271.png)

---

## Parameters

| **Parameter**      | **Description**                                                                                 | **Default Value** | **Parameter in Workflow File** | **Type**  |
|--------------------|-------------------------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| Result file        | Location of the output data file. If this is set, the `Location` slot in the port will not be used. | *(none)*          | *(not specified)*              | _string_  |
| Accumulate results | Accumulate all incoming data in one file or create separate files for each input (with suffix). | `false` (default) | *(not specified)*              | _boolean_ |
