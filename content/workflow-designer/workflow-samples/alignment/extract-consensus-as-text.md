---
title: "Extract Consensus as Text"
weight: 300
---

# Extract Consensus as Text

For each input multiple alignment, the workflow calculates the consensus and saves it to a plain text file, named
according to the input alignment name.

By default, the **JalView** algorithm (denoted as **"default"**) is used to calculate the consensus. For each alignment
column:

- If two characters have high frequency, a `"+"` symbol is inserted.
- Otherwise, a character is returned either in **uppercase** or **lowercase**, depending on the percentage value and the
  **threshold** parameter.

Alternatively, you can choose the **ClustalW** algorithm:

- `"*"` — all characters in the column are identical.
- `":"` — conserved between strongly similar properties (score > 0.5 in the Gonnet PAM 250 matrix).
- `"."` — conserved between weakly similar properties (score < 0.5).
- `" "` — no conservation.

> **Note:** The **threshold** parameter does **not apply** to the ClustalW algorithm.

---

## How to Use This Sample

If you haven't used the workflow samples in UGENE before,
see [How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows).

---

## Workflow Sample Location

This sample, **"Extract Consensus as Text"**, can be found in the **"Alignment"** section of the Workflow Designer
samples.

---

## Workflow Image

The opened workflow looks as follows:

![Workflow image](/images/65930239/65930240.png)

---

## Workflow Wizard

The wizard includes **3 pages**:

### 1. Input Multiple Alignments

On this page, you must input multiple alignment file(s).

![Input page](/images/65930239/65930241.png)

---

### 2. Extracting Consensus Settings

Modify the consensus extraction parameters here.

![Settings page](/images/65930239/65930242.png)

| **Parameter** | **Description**                                                        |
|---------------|------------------------------------------------------------------------|
| **Algorithm** | The algorithm used for consensus calculation (`default` or `ClustalW`) |
| **Threshold** | Percentage cutoff for JalView algorithm (ignored by ClustalW)          |

---

### 3. Output Files

Each input alignment produces a corresponding text file with the consensus string.

![Output page](/images/65930239/65930243.png)
