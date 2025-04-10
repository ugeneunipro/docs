---
title: "Read HMM2 Profile Element"
weight: 300
---

# Read HMM2 Profile Element

Reads HMM profiles from file(s). The files can be local or Internet URLs.

**Element type:** hmm2-read-profile

Parameters
----------

| Parameter        | Description                                        | Default value | Parameter in Workflow File | Type    |
|------------------|----------------------------------------------------|---------------|----------------------------|---------|
| **Input files** _(required)_ | Semicolon-separated list of paths to the input files. |               | url-in                     | _string_ |

Input/Output Ports
------------------

The element has 1 _output port_:

| Name in GUI       | Name in Workflow File | Type          |
|-------------------|-----------------------|---------------|
| **HMM profile**   | out-hmm2              | _hmm2-profile_ |

**Slots:**

| Slot In GUI     | Slot in Workflow File  | Type          |
|-----------------|------------------------|---------------|
| **HMM profile** | hmm2-profile           | _hmm2-profile_ |