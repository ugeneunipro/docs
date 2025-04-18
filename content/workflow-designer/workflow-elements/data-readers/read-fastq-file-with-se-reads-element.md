---
title: "Read FASTQ File with SE Reads Element"
weight: 300
---

# Read FASTQ File with SE Reads Element

Input one or several files with NGS single-end reads in FASTQ format. The element outputs the file(s) URL(s).

**Type:** get-se-reads-list

Parameters
----------

| Parameter       | Description | Default value | Parameter in Workflow File | Type    |
|-----------------|-------------|---------------|----------------------------|---------|
| **Input file(s)** | Input files. | Dataset 1   | **url1**                   | _string_ |

Input/Output Ports
------------------

The element has one _output port_:

| Name in GUI   | Name in Workflow File | Type    |
|---------------|-----------------------|---------|
| Output file   | out                   |         |

**Slots:**

| Slot In GUI     | Slot in Workflow File | Type    |
|-----------------|-----------------------|---------|
| Source URL 1    | **reads-url1**        | _string_ |