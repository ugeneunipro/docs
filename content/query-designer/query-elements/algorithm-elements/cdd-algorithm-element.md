---
title: "CDD Algorithm Element"
weight: 100
---


# CDD Algorithm Element

When the _element_ is used the input nucleotide sequence is translated into 6 amino sequences. The translated sequences are used to query the NCBI Conserved Domain Database (CDD).

Parameters in GUI
-----------------

Parameter

Description

Default value

**Annotate As**

Name of the result annotations.

CDD result

**Expected value**

It is also called E-value. Describes the number of hits one can “expect” to see by chance when searching a database of a particular size.

10

**Min length**

Minimum result length.

50bp

**Max length**

Maximum result length.

5000bp

**Pattern**

Filters the result annotations: the qualifier value must contain the specified pattern value.

No default value.

Parameters in Schema File
-------------------------

**Type:** CDD

Parameter

Parameter in the GUI

Type

**key**

**Annotate As**

_string_

**evalue**

**Expected value**

_numeric_

**min-length**

**Min length**

_numeric_

**max-length**

**Max length**

_numeric_

**pattern**

**Pattern**

_string_
