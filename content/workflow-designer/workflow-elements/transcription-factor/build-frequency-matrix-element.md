---
title: "Build Frequency Matrix Element"
weight: 100
---

# Build Frequency Matrix Element

Builds a frequency matrix. Frequency matrices are used for probabilistic recognition of transcription factor binding
sites.

**Element type:** fmatrix-build

## Parameters

| Parameter       | Description                                                                                             | Default value | Parameter in Workflow File | Type      |
|-----------------|---------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Matrix type** | Dinucleic matrices are more detailed, while mononucleic ones are more useful for small input data sets. | Mononucleic   | **type**                   | _boolean_ |

Available values are:

* `true` – for Dinucleic
* `false` – for Mononucleic

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input alignment_
**Name in Workflow File:** in-msa
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |

And 1 _output port_:

**Name in GUI:** _Frequency matrix_
**Name in Workflow File:** out-fmatrix
**Slots:**

| Slot In GUI          | Slot in Workflow File | Type      |
|----------------------|-----------------------|-----------|
| **Frequency matrix** | **fmatrix**           | _fmatrix_ |
