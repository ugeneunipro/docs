---
title: "Change Chromosome Notation for VCF Element"
weight: 200
---


# Change Chromosome Notation for VCF Element

Changes chromosome notation for each variant from the input, VCF or other variation files.

**Element type:** rename-chromosome-in-variation

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Replace prefixes**

Input the list of chromosome prefixes that you would like to replace. For example "NC\_000". Separate different prefixes by semicolons.



prefixes-to-replace

_string_

**Replace by**

Input the prefix that should be set instead, for example "chr".



prefix-replace-with

_string_

Input/Output Ports
------------------

The element has 1 _input ports_:

**Name in GUI:** Input file URL

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_

And 1 _output port_:

**Name in GUI:** Output file URL

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Produced URL**

**url**

_string_
