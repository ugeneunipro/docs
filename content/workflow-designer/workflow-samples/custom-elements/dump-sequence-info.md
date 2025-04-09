---
title: "Dump Sequence Info"
weight: 300
---

# Dump Sequence Info

This workflow dumps the sequence name and sequence size to output for all incoming sequences.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at
the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

---

### Workflow Sample Location

The workflow sample **"Dump Sequence Info"** can be found in the **"Custom Elements"** section of the Workflow Designer
samples.

---

### Workflow Image

The workflow looks as follows:

![Workflow image](/images/65930268/65930269.png)

---

### Workflow Wizard

The wizard has 2 pages.

#### 1. Input sequence(s)

On this page, you must input sequence(s).

![Input sequences](/images/65930268/65930270.png)

#### 2. Output data

On this page, you can modify output settings.

![Output data](/images/65930268/65930271.png)

---

## Parameters

| **Parameter**      | **Description**                                                                                 | **Default Value** | **Parameter in Workflow File** | **Type**  |
|--------------------|-------------------------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| Result file        | Location of output data file. If this is set, the `Location` slot in the port will not be used. | *(none)*          | *(not specified)*              | _string_  |
| Accumulate results | Accumulate all incoming data in one file or create separate files for each input (with suffix). | `false` (default) | *(not specified)*              | _boolean_ |
