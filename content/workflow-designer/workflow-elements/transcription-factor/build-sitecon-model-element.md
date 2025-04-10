---
title: "Build SITECON Model Element"
weight: 200
---

# Build SITECON Model Element

Builds a statistical profile for SITECON. SITECON is a program designed for the probabilistic recognition of transcription factor binding sites.

**Element type:** sitecon-build

## Parameters

| Parameter              | Description                                                                                                                                                                    | Default value | Parameter in Workflow File | Type      |
|------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Weight algorithm**   | An optional feature. In most cases, applying no weight will suffice. However, in some cases, choosing algorithm 2 may enhance recognition quality.                              | None          | **weight-algorithm**       | _boolean_ |
|                        | Available values are:<br>• `0` - for None<br>• `1` - for Algorithm2                                                                                                            |               |                            |           |
| **Window size, bp**    | A window used to identify the most important alignment region, located at the center of the alignment. Must not exceed the alignment length. Recommended: ≤ 50 bp.             | 40            | **window-size**            | _numeric_ |
| **Calibration length** | Length of random synthetic sequences used to calibrate the profile. Should not be less than the window size.                                                                   | 1M            | **calibrate-length**       | _numeric_ |
| **Random seed**        | A positive integer to generate reproducible results.                                                                                                                           | 0             | **seed**                   | _numeric_ |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input alignment_  
**Name in Workflow File:** in-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |
| **Origin**  | **url**               | _string_ |

And 1 _output port_:

**Name in GUI:** _Sitecon model_  
**Name in Workflow File:** out-sitecon  
**Slots:**

| Slot In GUI       | Slot in Workflow File | Type            |
|-------------------|-----------------------|-----------------|
| **Sitecon model** | **sitecon-model**     | _sitecon-model_ |