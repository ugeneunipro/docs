---
title: "Read HMM3 Profile"
weight: 300
---

# Read HMM3 Profile

This document describes how to read HMM3 profiles from files. The files can be accessed locally or via Internet URLs.

**Element type:** hmm3-read-profile

## Parameters

| Parameter      | Description                               | Default Value | Parameter in Workflow File | Type    |
|----------------|-------------------------------------------|---------------|----------------------------|---------|
| **Input files** (required) | Semicolon-separated list of paths to the input files. |               | url-in                     | _string_ |

## Input/Output Ports

The element has one _output port_:

- **Name in GUI:** _HMM3 profile_
- **Name in Workflow File:** out-hmm3

### Slots

| Slot In GUI   | Slot in Workflow File | Type          |
|---------------|-----------------------|---------------|
| **HMM profile** | **hmm3-profile**     | _hmm3-profile_ |