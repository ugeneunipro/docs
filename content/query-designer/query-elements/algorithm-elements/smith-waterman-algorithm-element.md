---
title: "Smith-Waterman Algorithm Element"
weight: 1100
---

# Smith-Waterman Algorithm Element

The _element_ uses the Smith-Waterman algorithm to search the input sequence for regions similar to the specified pattern.

Parameters in GUI
-----------------

| Parameter             | Description                                                                                   | Default Value     |
|-----------------------|-----------------------------------------------------------------------------------------------|-------------------|
| **Annotate As**       | Name of the result annotations.                                                              | misc_feature      |
| **Direction**         | See the description [_here_](../../manipulating-schema/managing-strands/element-direction-in-schema). | Any               |
| **Algorithm**         | Algorithm version. Depending on the computer configuration, the following values may be available: <ul><li>Classic 2</li><li>SSE2</li></ul> | Classic 2         |
| **Filter results**    | Results filtering strategy. The available values are: <ul><li>filter-intersections</li><li>none</li></ul> | filter-intersections |
| **Gap ext score**     | Gap extension score.                                                                         | -1.00             |
| **Gap open score**    | Gap open score.                                                                              | -10.00            |
| **Scoring matrix**    | Specifies the scoring matrix to use.                                                         | Auto              |
| **Min score**         | Percentage of matching between the pattern and the searched sequence region.                  | 90%               |
| **Pattern**           | The pattern to search for.                                                                   | You must specify a value! |
| **Search in translation** | Translates the nucleotide sequence supplied into a protein sequence and searches in the translated sequence. | False             |

Parameters in Schema File
-------------------------

**Type:** ssearch

| Parameter          | Parameter in the GUI        | Type     |
|--------------------|------------------------------|----------|
| **key**            | **Annotate As**              | _string_ |
| **algorithm**      | **Algorithm**                | _string_ |
|                    | Depending on the computer configuration, the available values are: <ul><li>“Classic 2”</li><li>SSE2</li></ul> |          |
| **filter**         | **Filter results**           | _string_ |
|                    | The available values are: <ul><li>filter-intersections</li><li>none</li></ul> |          |
| **gap-ext-score**  | **Gap ext score**            | _numeric_|
| **gap-open-score** | **Gap open score**           | _numeric_|
| **matrix**         | **Scoring matrix**           | _string_ |
| **min-score**      | **Min score**                | _numeric_|
| **pattern**        | **Pattern**                  | _string_ |
| **strand**         | **Direction**                | _string_ |
|                    | Available values are: <ul><li>complement</li><li>direct</li><li>both</li></ul> |          |
| **translate**      | **Search in translation**    | _boolean_ |