---
title: "Convert UQL Schema Results to Alignment"
weight: 300
---

# Convert UQL Schema Results to Alignment

This schema allows analyzing a sequence using a Query and saving the results as an alignment of selected features.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, check the
"[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

### Workflow Sample Location

The workflow sample **"Convert UQL Schema Results to Alignment"** can be found in the **"Conversions"** section of the
Workflow Designer samples.

### Workflow Image

The workflow looks as follows:

![](/images/65930255/65930256.png)

## Workflow Wizard

The wizard has 2 pages:

---

### 1. Input Sequence(s)

On this page, you must input the sequence(s).

![](/images/65930255/65930257.png)

---

### 2. Annotate with UQL

On this page, you can modify annotation and output settings.

![](/images/65930255/65930258.png)

| Parameter            | Description                                                                                            |
|----------------------|--------------------------------------------------------------------------------------------------------|
| **UQL schema file**  | Schema file.                                                                                           |
| **Merge**            | If set to true, merges regions of each result into a single annotation.                                |
| **Offset**           | Left and right offset to apply to merged annotations (if "Merge" is true).                             |
| **Annotation names** | File with annotation names (whitespace-separated) or list of annotation names to include/exclude.      |
| **Accept or filter** | Choose whether to accept only the specified annotation names or to filter them out.                    |
| **Result file**      | Location of the output data file. If this is set, it overrides the "Location" slot of the output port. |
| **Document format**  | Format of the output file.                                                                             |
