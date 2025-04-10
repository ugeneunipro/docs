---
title: "Find Pattern Element"
weight: 1000
---

# Find Pattern Element

Searches regions in a sequence that are similar to a pattern sequence. It outputs a set of annotations.

---

## Element Type

**Element type:** `search`

---

## Parameters

| **Parameter**                   | **Description**                                                              | **Default Value**  | **Parameter in Workflow File** | **Type**  |
|---------------------------------|------------------------------------------------------------------------------|--------------------|--------------------------------|-----------|
| Annotate as                     | Name of the result annotation                                                | `misc_feature`     | `result-name`                  | _string_  |
| Pattern(s)                      | Semicolon-separated list of patterns to search for                           |                    | `pattern`                      | _string_  |
| Pattern file                    | Load pattern from file in any sequence format or in newline-delimited format |                    | `pattern_file`                 | _string_  |
| Use pattern name                | Use names from pattern file as annotation names                              | `False`            | `use-names`                    | _boolean_ |
| Max Mismatches                  | Maximum allowed mismatches between substring and pattern                     | `0`                | `max-mismatches-num`           | _numeric_ |
| Search in                       | Strand(s) to search: 0 = both, 1 = direct, 2 = complement                    | `both strands (0)` | `strand`                       | _numeric_ |
| Allow Insertions/Deletions      | Allow indels when searching                                                  | `False`            | `allow-ins-del`                | _boolean_ |
| Support ambiguous bases         | Enables ambiguous base handling (disables indels)                            | `False`            | `ambiguous`                    | _boolean_ |
| Search in Translation           | Translate nucleotide sequence to protein and search in protein sequence      | `False`            | `amino`                        | _boolean_ |
| Qualifier name for pattern name | Name of qualifier used to store pattern name in the result annotations       | `pattern_name`     | `pattern-name-qual`            | _string_  |

---

## Input/Output Ports

### Input Port

| **Name in GUI** | **Name in Workflow File** | **Slot**   | **Slot in Workflow File** | **Type**   |
|-----------------|---------------------------|------------|---------------------------|------------|
| Input data      | `in-sequence`             | Sequence   | `sequence`                | _sequence_ |
|                 |                           | Plain text | `text`                    | _string_   |

### Output Port

| **Name in GUI**     | **Name in Workflow File** | **Slot**           | **Slot in Workflow File** | **Type**           |
|---------------------|---------------------------|--------------------|---------------------------|--------------------|
| Pattern annotations | `out-annotations`         | Set of annotations | `annotations`             | _annotation-table_ |

---

This element is useful for detecting motifs or other predefined nucleotide or protein patterns in biological sequences
with support for flexible matching and ambiguity handling.