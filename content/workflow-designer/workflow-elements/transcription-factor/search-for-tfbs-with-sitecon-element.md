---
title: "Search for TFBS with SITECON Element"
weight: 800
---


# Search for TFBS with SITECON Element

Searches each input sequence for transcription factor binding sites significantly similar to specified SITECON profiles. In case several profiles were supplied, searches with all profiles one by one and outputs merged set of annotations for each sequence.

**Element type:** sitecon-search

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Result annotation**

Name of the result annotations.

misc\_feature

**result-name**

_string_

**Search in**

Specifies which strands should be searched: direct, complement or both.

both strands

**strand**

_numeric_

Available values are:

*   0 - for searching in both strands
*   1 - for searching in direct strand
*   2 - for searching in complement strand

**Min score**

Recognition quality threshold, should be less than 100%. Choosing too low threshold will lead to recognition of too many TFBS recognised with too low trustworthiness. Choosing too high threshold may result in no TFBS recognised.

85

**min-score**

_numeric_

**Min err1**

Alternative setting for filtering results, minimal value of Error type I. Note that all thresholds (by score, by err1 and by err2) are applied when filtering results.

0.0

**err1**

_numeric_

**Max err2**

Alternative setting for filtering results, max value of Error type II. Note that all thresholds (by score, by err1 and by err2) are applied when filtering results.

0.001

**err2**

_numeric_

Input/Output Ports

The element has 2 _input ports_. The first port:

**Name in GUI:** _Sequence_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

The second input port gets the SITECON model:

**Name in GUI:** _Sitecon model_

**Name in Workflow File:** in-sitecon

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sitecon model**

**sitecon-model**

_sitecon-model_

And there is 1 _output port_:

**Name in GUI:** _Sitecon annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
