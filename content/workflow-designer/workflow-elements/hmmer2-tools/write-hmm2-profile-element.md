---
title: "Write HMM2 Profile Element"
weight: 400
---

# Write HMM2 Profile Element

Saves all input HMM profiles to the specified locations.

**Element type:** hmm2-write-profile

## Parameters

| Parameter         | Description                                                                                                                                             | Default value | Parameter in Workflow File | Type          |
|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|---------------|
| **Output file**   | Location of the output data file. If this attribute is set, the “Location” slot is not taken into account.                                               |               | **url-out**                | _string_      |
| **Existing file** | If a target file already exists, you can specify how it should be handled: either overwritten, renamed, or appended (if supported by the file format).  | Rename        | **write-mode**             | _numeric_     |

Available values for **Existing file** are:
- 0 - for overwrite
- 1 - for append
- 2 - for rename

## Input/Output Ports

The element has 1 _input port_:

| Name in GUI      | Name in Workflow File | Type          |
|------------------|-----------------------|---------------|
| **HMM profile**  | in-hmm2               | _hmm2-profile_|

**Slots:**

| Slot In GUI     | Slot in Workflow File | Type     |
|-----------------|-----------------------|----------|
| **HMM profile** | **hmm2-profile**      | _hmm2-profile_ |
| **Location**    | **url**               | _string_ |