---
title: "Read Frequency Matrix Element"
weight: 500
---

# Read Frequency Matrix Element

This element is used to read frequency matrices from files. The files can be either local or accessed via Internet URLs.

**Element type:** fmatrix-read

## Parameters

| Parameter     | Description                                      | Default value | Parameter in Workflow File | Type     |
|---------------|--------------------------------------------------|---------------|----------------------------|----------|
| **Input files** (required) | Semicolon-separated list of paths to the input files. |               | url-in                     | _string_ |

## Input/Output Ports

The element has one _output port_:

| Slot In GUI        | Slot in Workflow File | Type     |
|--------------------|-----------------------|----------|
| **Frequency matrix** | fmatrix               | _fmatrix_ |

- **Name in GUI:** _Frequency matrix_
- **Name in Workflow File:** out-fmatrix