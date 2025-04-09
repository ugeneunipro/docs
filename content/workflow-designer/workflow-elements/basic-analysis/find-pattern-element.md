---
title: "Find Pattern Element"
weight: 1000
---


# Find Pattern Element

Searches regions in a sequence similar to a pattern sequence. Outputs a set of annotations.

**Element type:** search

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Annotate as**

Name of the result annotation.

misc\_feature

**result-name**

_string_

**Pattern(s)**

Semicolon-separated list of patterns to search for.



**pattern**

_string_

**Pattern file**

Load pattern from file in any sequence format or in newline-delimited format.



**pattern\_file**

_string_

**Use pattern name**

If patterns are loaded from a file, use names of pattern sequences as annotation names. The name from the parameters is used by default.

False

**use-names**

_boolean_

**Max Mismatches**

Maximum number of mismatches between a substring and a pattern.

0

**max-mismatches-num**

_numeric_

**Search in**

Specifies which strands should be searched: direct, complementary or both.

both strands

**strand**

_numeric_

Available values are:

*   0 - for searching in both strands
*   1 - for searching in direct strand
*   2 - for searching in complement strand

**Allow Insertions/Deletions**

Takes into account possibility of insertions/deletions when searching. By default substitutions are only considered.

False

**allow-ins-del**

_boolean_

**Support ambiguous bases**

Performs correct handling of ambiguous bases. When this option is activated insertions and deletions are not considered.

False

**ambiguous**

_boolean_

**Search in Translation**

Translates a supplied nucleotide sequence to protein and searches in the translated sequence.

False

**amino**

_boolean_

**Qualifier name for pattern name**

Name of qualifier in result annotations which is containing a pattern name.

pattern\_name

**pattern-name-qual**

_string_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input data_

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

**Plain text**

**text**

_string_

And 1 _output port_:

**Name in GUI:** _Pattern annotations_

**Name in Workflow File:** out-annotations

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_
