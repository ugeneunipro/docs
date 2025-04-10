---
title: "Read SITECON Model Element"
weight: 600
---

# Read SITECON Model Element

Reads SITECON profiles from files. The files can be local or Internet URLs.

**Element type:** sitecon-read

## Parameters

| Parameter          | Description                                      | Default Value | Parameter in Workflow File | Type   |
|--------------------|--------------------------------------------------|---------------|----------------------------|--------|
| **Input files**    | A semicolon-separated list of paths to the input files. |               | **url-in**                 | _string_ |

## Input/Output Ports

The element has 1 _output port_:

| Name in GUI      | Name in Workflow File | Type            |
|------------------|-----------------------|-----------------|
| **Sitecon model** | out-sitecon           | _sitecon-model_ |