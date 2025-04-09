---
title: "Generate DNA Element"
weight: 200
---


# Generate DNA Element

Generates random DNA sequences with given nucleotide content that can be specified manually or evaluated from the reference file.

**Element type:** generate-dna

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Length**

Length of the resulted sequence or sequences.

1000 bp

**length**

_numeric_

**Count**

Number of sequences to generate.

1

**count**

_numeric_

**Seed**

Value to initialize the random generator. By default (seed = -1) the generator is initialized with the system time.

\-1

**seed**

_numeric_

**Content**

Specifies how the nucleotide content of the sequence(s) should be generated. It can be either taken from the reference file (see the _Reference_parameter), or input manually.

manual

**content**

_string_

**Algorithm**

Algorithm for generating random sequence(s). Two algorithms are available: GC Content and GC Skew. If you choose GC Content, then parameters _A_,_C_, _G_, _T_ are used to generate the sequence. Otherwise, the _GC Skew_parameter is used to generate the sequence(s).

GC Content

**algorithm**

_string_

Available values are:

*   gc-content
*   gc-skew

**Window size**

The DNA sequence generation is divided into windows of the specified size. In each window the bases ratio, defined by other parameters, is kept.

1000

**window-size**

_numeric_

**Reference**

Path to the reference file (could be a sequence or an alignment).



**reference-url**

_string_

Available values are:

*   manual
*   reference

**A**

Adenine content.

25%

**percent-a**

_numeric_

**C**

Cytosine content.

25%

**percent-c**

_numeric_

**G**

Guanine content.

25%

**percent-g**

_numeric_

**T**

Thymine content.

25%

**percent-t**

_numeric_

**GC Skew**

GC Skew is calculated as (G - C) / (G + C), where G is the number of G’s in the window, and C is the number of C’s.

0.25

**gc-skew**

_numeric_

Input/Output Ports

The element has 1 _output port_:

**Name in GUI:** _Sequences_

**Name in Workflow File:** out-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_
