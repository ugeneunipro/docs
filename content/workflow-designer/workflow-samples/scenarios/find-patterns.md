---
title: "Find Patterns"
weight: 300
---

# Find Patterns

This simple workflow finds patterns in your sequences and saves them as annotations. You can use the workflow to map primers, regulatory signals, genes, etc. It loads any set of sequences from your files or folders and finds patterns in them.

---

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the ["How to Use Sample Workflows"](../../introduction/how-to-use-sample-workflows) section of the documentation.

---

## Workflow Sample Location

The workflow sample **"Find Patterns"** can be found in the **"Scenarios"** section of the Workflow Designer samples.

---

## Workflow Image

The workflow looks as follows:

![Workflow](/images/65930540/65930541.png)

---

## Workflow Wizard

The wizard has 3 pages:

---

### 1. Input Sequence(s)

On this page, you must input sequence(s).

![Input](/images/65930540/65930542.png)

---

### 2. Find Pattern

On this page, you must input pattern(s) and you can modify the search parameters.

![Pattern Settings](/images/65930540/65930543.png)

#### Available Parameters

| **Parameter**                  | **Description**                                                                                 |
|--------------------------------|-------------------------------------------------------------------------------------------------|
| **Pattern**                    | A semicolon-separated list of patterns to search for.                                           |
| **Annotate as**                | Name of the resulting annotations.                                                              |
| **Use pattern name**           | If patterns are loaded from a file, use the names of the pattern sequences as annotation names. |
| **Max Mismatches**             | Maximum number of mismatches between a substring and a pattern.                                 |
| **Allow Insertions/Deletions** | Allow insertions or deletions when searching. By default, only substitutions are considered.    |
| **Search in Translation**      | Translate the supplied nucleotide sequence to protein and search in the translated sequence.    |
| **Support ambiguous bases**    | Handle ambiguous bases (e.g. N, R, Y) properly. Disables insertions/deletions when enabled.     |
| **Qualifier name**             | Name of the qualifier in result annotations that contains the pattern name.                     |

---

### 3. Output Data

On this page, you can modify the output parameters.

![Output](/images/65930540/65930544.png)