---
title: "SITECON Algorithm Element"
weight: 1000
---

# SITECON Algorithm Element

The _element_ searches the input sequence for transcription factor binding sites (TFBSs) that are significantly similar to the specified SITECON profiles.

Parameters in GUI
-----------------

| Parameter       | Description                                                                                                         | Default value |
|-----------------|---------------------------------------------------------------------------------------------------------------------|---------------|
| **Annotate As** | Name of the result annotations.                                                                                      | misc\_feature |
| **Direction**   | See the description [_here_](../../manipulating-schema/managing-strands/element-direction-in-schema).                | Any           |
| **Min Err1**    | Filters the results by minimum value of Error type I.                                                                | 0             |
| **Max Err2**    | Filters the results by maximum value of Error type II.                                                               | 0.001         |
| **Model**       | Semicolon-separated list of SITECON profiles. You must specify a value!                                              |               |
| **Min score**   | Recognition quality percentage threshold. Choosing too low a threshold will lead to recognition of too many TFBS. Choosing too high a threshold will result in no TFBS recognized. | 85%           |

Parameters in Schema File
-------------------------

**Type:** sitecon

| Parameter | Parameter in the GUI | Type     |
|-----------|----------------------|----------|
| **key**   | **Annotate As**      | _string_ |
| **err1**  | **Min Err1**         | _numeric_|
| **err2**  | **Max Err2**         | _numeric_|
| **profile** | **Model**          | _string_ |
| **score** | **Min score**        | _numeric_|
| **strand** | **Direction**       | _string_ |

Available values are:

- complement
- direct
- both