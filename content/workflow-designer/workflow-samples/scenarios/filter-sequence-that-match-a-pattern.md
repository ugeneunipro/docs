---
title: "Filter Sequence That Match a Pattern"
weight: 100
---

# Filter Sequence That Match a Pattern

This workflow allows filtering sequences that match (or do not match) user-specified patterns.

---

## How to Use This Sample

If you haven't used workflow samples in UGENE before, refer to
the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

---

## Workflow Sample Location

The workflow sample **"Filter Sequence That Match a Pattern"** is available in the **Scenarios** section of the Workflow
Designer samples.

---

## Workflow Image

The workflow looks as follows:

![](/images/65930530/65930531.png)

---

## Workflow Wizard

The wizard consists of 3 pages:

### 1. Input sequence(s)

On this page, input sequence files must be selected.

![](/images/65930530/65930532.png)

---

### 2. Find pattern

On this page, patterns must be specified, and search parameters can be configured.

![](/images/65930530/65930533.png)

#### Parameters

| **Parameter**              | **Description**                                                               | **Default Value** | **Type**  |
|----------------------------|-------------------------------------------------------------------------------|-------------------|-----------|
| Pattern                    | Semicolon-separated list of patterns to search for                            | *(user-defined)*  | _string_  |
| Use pattern name           | Use names of pattern sequences as annotation names (if loaded from file)      | False             | _boolean_ |
| Max Mismatches             | Maximum number of mismatches allowed between a substring and a pattern        | 0                 | _numeric_ |
| Allow Insertions/Deletions | Consider insertions/deletions in search                                       | False             | _boolean_ |
| Search in Translation      | Translate nucleotide sequence to protein and search in translated sequence    | False             | _boolean_ |
| Support ambiguous bases    | Handle ambiguous bases correctly (disables insertions/deletions when enabled) | False             | _boolean_ |
| Qualifier name             | Name of the qualifier in result annotations containing the pattern name       | pattern           | _string_  |

---

### 3. Output data

This page allows configuring the output file.

![](/images/65930530/65930534.png)
