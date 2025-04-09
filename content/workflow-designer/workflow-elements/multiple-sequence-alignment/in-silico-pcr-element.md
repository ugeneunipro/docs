---
title: "In Silico PCR Element"
weight: 1000
---


# In Silico PCR Element

Simulates PCR for input sequences and primer pairs. Creates the table with the PCR statistics.

**Element type:** in-silico-pcr

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Primers URL**

A URL to the input file with primer pairs.



**primers-url**

_string_

**Report URL**

A URL to the output file with the PCR report.



**report-url**

_string_

**Mismatches**

Number of allowed mismatches.

3

**mismatches**

_numeric_

**Min perfect match**

Number of bases that match exactly on 3' end of primers.

15

**perfect-match**

_numeric_

**Max product size**

Maximum size of amplified region.

5000

**max-product**

_numeric_

**Use ambiguous bases**

Search for ambiguous bases (as \\"N\\") if checked.

True

**use-ambiguous-bases**

_boolean_

**Extract annotations**

Extract annotations within a product region.

Inner

**extract-annotations**

_string_



Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input sequence

**Name in Workflow File:** in-sequence

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Sequence**

**sequence**

_sequence_

And 1 _output port_:

**Name in GUI:** PCR product

**Name in Workflow File:** out

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Set of annotations**

**annotations**

_annotation-table_

**Sequence**

**sequence**

_sequence_
