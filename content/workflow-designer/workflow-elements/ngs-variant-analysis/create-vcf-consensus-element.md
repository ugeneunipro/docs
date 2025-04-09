---
title: "Create VCF Consensus Element"
weight: 400
---

# Create VCF Consensus Element

Apply VCF variants to a FASTA file to create a consensus sequence.

**Element type:** vcf-consensus

## Parameters

| Parameter                  | Description                                              | Default value | Parameter in Workflow File | Type     |
|----------------------------|----------------------------------------------------------|---------------|----------------------------|----------|
| **Output FASTA consensus** | The URL to the output file with the resulting consensus. |               | **consensus-url**          | _string_ |

## Input/Output Ports

| Port Name (GUI)         | Workflow File Name | Slots                                                                |
|-------------------------|--------------------|----------------------------------------------------------------------|
| **Input FASTA and VCF** | `in-data`          | **Fasta url** → `fasta` (_string_)<br>**VCF url** → `vcf` (_string_) |
| **Fasta consensus URL** | `out-consensus`    | **out-consensus** → `out-consensus` (_string_)                       |
