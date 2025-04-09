---
title: "Convert Frequency Matrix Element"
weight: 400
---


# Convert Frequency Matrix Element

Converts a frequency matrix to a weight matrix. Weight matrices are used for probabilistic recognition of transcription factor binding sites.

**Element type:** fmatrix-to-wmatrix

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Matrix type** (required)

Dinucleic matrices are more detailed, while mononucleic one is more useful for small input data sets.

Mononucleic

**type**

_boolean_

Available values are:

*   true - for Dinucleic
*   false - for Mononucleic

**Weight algorithm**

Different weight algorithms use different functions to build weight matrices. It allows us to get better precision on different data sets. Log-odds, NLG and Match algorithms are sensitive to input matrices with zero values, so some of them may not work on those matrices.

Berg and Von Hippel

**weight-algorithm**

_string_

Available values are:

*   Berg and von Hippel
*   Log-odds
*   Match
*   NLG

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Frequency matrix_

**Name in Workflow File:** in-fmatrix

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Frequency matrix**

**fmatrix**

_fmatrix_

And 1 _output port_:

**Name in GUI:** _Weight matrix_

**Name in Workflow File:** out-wmatrix

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Weight matrix**

**wmatrix**

_wmatrix_
