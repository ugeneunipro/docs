---
title: "Convert SnpEff Variations to Annotations Element"
weight: 300
---

# Convert SnpEff Variations to Annotations Element

Parses information added to variations by SnpEff into standard annotations.

**Element type:** convert-snpeff-variations-to-annotations

## Parameters

| Parameter           | Description                                                                             | Default value | Parameter in Workflow File | Type     |
|---------------------|-----------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Output file**     | Location of the output data file. If set, overrides the "Location" slot of the output port. |               | **url-out**                | _string_ |
| **Document format** | Format of the output file.                                                              | genbank       | **document-format**        | _string_ |

## Input/Output Ports

| Port Name (GUI)    | Workflow File Name  | Slots                             |
|--------------------|---------------------|-----------------------------------|
| **Input file URL** | `in-variations-url` | **Source URL** → `url` (_string_) |