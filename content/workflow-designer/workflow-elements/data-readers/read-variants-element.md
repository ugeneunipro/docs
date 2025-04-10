---
title: "Read Variants Element"
weight: 1000
---

# Read Variants Element

Input one or several files with variants in one of the formats supported by UGENE (e.g., VCF).

The element outputs messages with the variant data.

See the list of all available formats [here](https://ugene.net/wiki/display/UUOUM27/Appendix+A.+Supported+File+Formats).

**Element type:** read-variations

## Parameters

| Parameter         | Description      | Default value | Parameter in Workflow File | Type     |
|-------------------|------------------|---------------|----------------------------|----------|
| **Input file(s)** | Input file(s).   | Dataset 1     | **url-in**                 | _string_ |

## Input/Output Ports

The element has 1 _output port_:

**Name in GUI:** Variation track  
**Name in Workflow File:** out-variations

| Slot In GUI       | Slot in Workflow File | Type        |
|-------------------|-----------------------|-------------|
| **Dataset name**  | **dataset**           | _string_    |
| **Source url**    | **url**               | _string_    |
| **Variation track** | **variation-track** | _variation_ |