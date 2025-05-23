---
title: "Align with MAFFT Element"
weight: 500
---

# Align with MAFFT Element

Originally, MAFFT is a multiple sequence alignment program for Unix-like operating systems. Currently, a Windows version
is also available.

MAFFT is used as an external tool from UGENE and it must be installed on your system. To learn more about external
tools, please read the main [UGENE User Manual](http://ugene.unipro.ru/documentation.html).

**Element type:** mafft

## Parameters

| Parameter               | Description                                                                               | Default value | Parameter in Workflow File | Type      |
|-------------------------|-------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Offset**              | Works like gap extension penalty.                                                         | 0             | **gap-ext-penalty**        | _numeric_ |
| **Gap open penalty**    | Gap open penalty.                                                                         | 1.53          | **gap-open-penalty**       | _numeric_ |
| **Max iteration**       | Maximum number of iterative refinements.                                                  | 0             | **iterations-max-num**     | _numeric_ |
| **Tool path** (default) | Path to the ClustalW tool. The default path can be set in the UGENE application settings. | default       | **path**                   | _string_  |
| **Temporary directory** | Directory to store temporary files.                                                       | default       | **temp-dir**               | _string_  |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input MSA_  
**Name in Workflow File:** in-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |

And 1 _output port_:

**Name in GUI:** _Multiple sequence alignment_  
**Name in Workflow File:** out-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type  |
|-------------|-----------------------|-------|
| **MSA**     | **msa**               | _msa_ |