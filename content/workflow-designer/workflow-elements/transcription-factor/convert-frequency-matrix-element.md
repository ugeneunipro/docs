---
title: "Convert Frequency Matrix Element"
weight: 400
---

# Convert Frequency Matrix Element

Converts a frequency matrix to a weight matrix.
Weight matrices are used for probabilistic recognition of transcription factor binding sites.

**Element type:** fmatrix-to-wmatrix

## Parameters

| Parameter            | Description                                                                                          | Default value       | Parameter in Workflow File | Type      |
|----------------------|------------------------------------------------------------------------------------------------------|---------------------|----------------------------|-----------|
| **Matrix type**      | Dinucleic matrices are more detailed, mononucleic are more useful for small datasets. **(Required)** | Mononucleic         | **type**                   | _boolean_ |
|                      | Available values:<br>• `true` – Dinucleic<br>• `false` – Mononucleic                                 |                     |                            |           |
| **Weight algorithm** | Weighting function to convert frequency matrix. Some are sensitive to zero values in input.          | Berg and Von Hippel | **weight-algorithm**       | _string_  |
|                      | Available values:<br>• `Berg and von Hippel`<br>• `Log-odds`<br>• `Match`<br>• `NLG`                 |                     |                            |           |

## Input/Output Ports

| Port Name (GUI)      | Workflow File Name | Slots                                        |
|----------------------|--------------------|----------------------------------------------|
| **Frequency matrix** | `in-fmatrix`       | **Frequency matrix** → `fmatrix` (_fmatrix_) |
| **Weight matrix**    | `out-wmatrix`      | **Weight matrix** → `wmatrix` (_wmatrix_)    |
