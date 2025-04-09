---
title: "Extract Consensus from Assembly"
weight: 300
---

# Extract Consensus from Assembly

The workflow sample below uses input assemblies to extract consensus sequences and saves them to FASTA files.

---

## How to Use This Sample

If you haven't used workflow samples in UGENE before, see
the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

---

## Workflow Sample Location

The sample **"Extract Consensus from Assembly"** can be found in the **"NGS"** section of the Workflow Designer samples.

---

## Workflow Image

The opened workflow looks like this:

![](/images/65930342/65930343.png)

---

## Workflow Wizard

The wizard has **1 page**:

### 1. Extract Consensus Page

On this page, you must:

- Input an assembly file
- Select an output file
- Optionally modify other input parameters

![](/images/65930342/65930344.png)

---

## Available Parameters

| **Parameter**    | **Description**                                                               |
|------------------|-------------------------------------------------------------------------------|
| **Assembly**     | Semicolon-separated list of paths to the input files.                         |
| **Algorithm**    | The algorithm used for consensus extraction.                                  |
| **Keep gaps**    | Set this to `True` if the resulting consensus must preserve gaps.             |
| **Output files** | Path to the output file. If set, the `Location` slot in the port is not used. |
