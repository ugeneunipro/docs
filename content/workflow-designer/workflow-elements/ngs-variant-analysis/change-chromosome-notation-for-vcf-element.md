---
title: "Change Chromosome Notation for VCF Element"
weight: 200
---

# Change Chromosome Notation for VCF Element

Changes chromosome notation for each variant from the input VCF or other variation files.

**Element type:** rename-chromosome-in-variation

## Parameters

| Parameter            | Description                                                                                           | Default value | Parameter in Workflow File | Type     |
|----------------------|-------------------------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Replace prefixes** | Input the list of chromosome prefixes to replace (e.g., `NC_000`). Separate multiple values with `;`. |               | **prefixes-to-replace**    | _string_ |
| **Replace by**       | Input the prefix to use instead (e.g., `chr`).                                                        |               | **prefix-replace-with**    | _string_ |

## Input/Output Ports

| Port Name (GUI)     | Workflow File Name | Slots                               |
|---------------------|--------------------|-------------------------------------|
| **Input file URL**  | `in-file`          | **Source URL** → `url` (_string_)   |
| **Output file URL** | `out-file`         | **Produced URL** → `url` (_string_) |
