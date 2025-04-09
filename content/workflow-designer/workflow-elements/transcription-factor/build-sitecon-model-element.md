---
title: "Build SITECON Model Element"
weight: 200
---


# Build SITECON Model Element

Builds statistical profile for SITECON. The SITECON is a program for probabilistic recognition of transcription factor binding sites.

**Element type:** sitecon-build

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Weight algorithm**

Optional feature, in most cases applying no weight will fit. In some cases choosing algorithm 2 will increase the recognition quality.

None

**weight-algorithm**

_boolean_

Available values are:

*   0 - for None
*   1 - for Algorithm2

**Window size, bp**

Window is used to pick out the most important alignment region and is located at the center of the alignment. Must be: windows size is not greater than TFBS alignment length, recommended: windows size is not greater than 50 bp.

40

**window-size**

_numeric_

**Calibration length**

Length of random synthetic sequences used to calibrate the profile. Should not be less than window size.

1M

**calibrate-length**

_numeric_

**Random seed**

The random seed, where is a positive integer. You can use this option to generate reproducible results for different runs on the same data.

0

**seed**

_numeric_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input alignment_

**Name in Workflow File:** in-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_

**Origin**

**url**

_string_

And 1 _output port_:

**Name in GUI:** _Sitecon model_

**Name in Workflow File:** out-sitecon

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sitecon model**

**sitecon-model**

_sitecon-model_
