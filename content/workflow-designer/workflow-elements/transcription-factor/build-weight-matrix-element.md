---
title: "Build Weight Matrix Element"
weight: 300
---

# Build Weight Matrix Element

Builds a weight matrix. Weight matrices are used for probabilistic recognition of transcription factor binding sites.

**Element type:** wmatrix-build

## Parameters

| Parameter                  | Description                                                                                                                | Default value       | Parameter in Workflow File | Type      |
|----------------------------|----------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------------|-----------|
| **Matrix type** (required) | Dinucleotide matrices are more detailed, while mononucleotide ones are more useful for small input data sets.              | Mononucleic         | **type**                   | _boolean_ |
|                            | Available values are:<br>• `true` – for Dinucleotide<br>• `false` – for Mononucleotide                                     |                     |                            |           |
| **Weight algorithm**       | Different weight algorithms use different functions to build weight matrices. Some may not work on matrices with zero values.| Berg and Von Hippel | **weight-algorithm**       | _string_  |
|                            | Available values are:<br>• Berg and von Hippel<br>• Log-odds<br>• Match<br>• NLG                                           |                     |                            |           |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input alignment_  
**Name in Workflow File:** in-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |

And 1 _output port_:

**Name in GUI:** _Weight matrix_  
**Name in Workflow File:** out-wmatrix  
**Slots:**

| Slot In GUI       | Slot in Workflow File | Type      |
|-------------------|-----------------------|-----------|
| **Weight matrix** | **wmatrix**           | _wmatrix_ |