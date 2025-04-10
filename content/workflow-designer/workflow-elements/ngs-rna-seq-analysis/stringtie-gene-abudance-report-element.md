---
title: "StringTie Gene Abundance Report Element"
weight: 500
---

# StringTie Gene Abundance Report Element

The element summarizes the gene abundance output of StringTie and saves the result into a common tab-delimited text file. The first two columns of the file are "Gene ID" and "Gene name". Each other column contains "FPKM" values for the genes from an input gene abundance file.

**Element type:** stringtie-gene-abundance-report

| Parameter     | Description                                  | Default value | Parameter in Workflow File | Type   |
|---------------|----------------------------------------------|---------------|----------------------------|--------|
| **Output file** | Specify the name of the output tab-delimited text file. |               | output-url                 | _string_ |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Input StringTie gene abundance file(s) URL

**Name in Workflow File:** in

| Slot in GUI   | Slot in **Workflow** File | Type   |
|---------------|---------------------------|--------|
| **Input URL** | url                       | _string_ |