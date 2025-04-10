---
title: "Find Substrings in Sequences"
weight: 100
---

# Find Substrings in Sequences

This sample workflow shows how to find substrings in input sequences, annotate them, and merge the found substring annotations with the original sequence annotations.

## Workflow Steps

1. The workflow reads sequences from the input sequence files (e.g., GenBank). The input data may also contain annotations associated with the sequences.
2. The workflow reads text strings (patterns) from the input text files.
3. The data are multiplexed using the [Multiplexer](../../workflow-elements/data-flow/multiplexer-element) element. A "1 to many" multiplexing rule is used, so each input sequence is concatenated with each pattern. The results are sent to the _Find Substrings_ element.
4. The _Find Substrings_ element searches for the specified patterns in each sequence.
5. The [Grouper](../../workflow-elements/data-flow/grouper-element) merges annotations from the input with those found by the _Find Substrings_ element. Grouping is done by sequence ID.
6. The merged data are saved to the output file (e.g., `substrings.gb`).

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, see: [How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows).

## Workflow Sample Location

The workflow sample "Find Substrings at Sequences" is in the "Data Merging" section of the Workflow Designer samples.

## Workflow Image

![](/images/65930287/65930288.png)

---

## Workflow Wizard

The wizard has 3 pages.

### 1. Input Sequences

You must provide the input sequence file(s):

![](/images/65930287/65930289.png)

### 2. Input Patterns

You must provide the input pattern(s):

![](/images/65930287/65930290.png)

### 3. Find Substrings

You can modify search and output parameters:

![](/images/65930287/65930291.png)

### Parameters

| **Parameter**                  | **Description**                                                                 |
|--------------------------------|---------------------------------------------------------------------------------|
| **Annotate as**                | Name of the result annotations.                                                 |
| **Allow Insertions/Deletions** | Consider insertions/deletions in pattern matching.                              |
| **Search in Translation**      | Translate nucleotide sequence to protein and search in translated sequence.     |
| **Support ambiguous bases**    | Properly handle ambiguous bases. Disables indel search when enabled.            |
| **Qualifier name**             | Name of the qualifier that contains the pattern name in result annotations.     |
| **Max Mismatches**             | Maximum allowed mismatches between substring and pattern.                       |
| **Result file**                | Location of the output file. If set, the port slot "Location" is ignored.       |
| **Accumulate results**         | Write all data to a single file or create separate files with numeric suffixes. |