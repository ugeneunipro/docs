---
title: "ORF Algorithm Element"
weight: 1
---


# ORF Algorithm Element

The _element_ searches for open reading frames (ORFs) in the supplied sequence.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Annotate As**

Name of the result annotations.

ORF

**Direction**

See the description [_here_](element-direction-in-schema.md).

Any

**Allow alternative codons**

Allows / disallows ORFs starting with alternative initiation codons, accordingly to the current translation table.

False

**Require init codons**

Allows / disallows ORFs starting with any codon other than terminator.

True

**Require stop codons**

Ignores or takes into account boundary ORFs which last beyond the search region.

False

**Min length**

Ignores ORFs shorter than the specified length.

100bp

**Max length**

Maximum length of annotation allowed.

10000bp

**Genetic code**

Genetic code that should be used to translate the input nucleotide sequence.

The standard genetic code

Parameters in Schema File
-------------------------

**Type:** orf

Parameter

Parameter in the GUI

Type

**key**

**Annotate As**

_string_

**strand**

**Direction**

_string_

Available values are:

*   complement
*   direct
*   both

**alt-start**

**Allow alternative codons**

_boolean_

**starts-with-init**

**Require init codons**

_boolean_

**ends-with-stop**

**Require stop codons**

_boolean_

**min-length**

**Min length**

_numeric_

**max-length**

**Max length**

_numeric_

**trans-id**

**Genetic code**

_string_

Available values are:

*   “NCBI-GenBank #1”
*   “NCBI-GenBank #2”
*   etc.
