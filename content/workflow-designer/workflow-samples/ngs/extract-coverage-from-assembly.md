---
title: "Extract Coverage from Assembly"
weight: 400
---

# Extract Coverage from Assembly

This workflow sample extracts **coverage** and/or **base counts** from input assemblies. It supports multiple input assemblies and produces a tab-delimited plain text output for each of them. Coverage values are filtered based on the provided threshold parameter.

---

## How to Use This Sample

If you haven't used workflow samples in UGENE before, refer to the [How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows) section of the documentation.

---

## Workflow Sample Location

The workflow sample **"Extract Coverage from Assembly"** is available in the **"NGS"** section of the Workflow Designer samples.

---

## Workflow Image

The workflow appears as follows:

![Workflow Image](/images/65930345/65930346.png)

---

## Workflow Wizard

The wizard consists of **3 pages**:

---

### 1. Input Assembly(ies)

On this page, input one or more assembly files.

![Input Page](/images/65930345/65930347.png)

---

### 2. Extract Parameters

Configure the extraction parameters:

![Extract Parameters Page](/images/65930345/65930348.png)

| **Parameter** | **Description**                                  |
|---------------|--------------------------------------------------|
| **Format**    | Output file format (tab-delimited plain text).   |
| **Export**    | Type of data to export: coverage or base counts. |
| **Threshold** | Minimum coverage value to include in the output. |

---

### 3. Output Data

On this page, select the destination for the output file.

![Output Page](/images/65930345/65930349.png)

---

## Output Example

Each output file will contain coverage data per base or region, based on the selected export mode and threshold.