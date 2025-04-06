---
title: "Create VCF Consensus Element"
weight: 1
---


# Create VCF Consensus Element

Apply VCF variants to a fasta file to create a consensus sequence.

**Element type:** vcf-consensus

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output FASTA consensus**

The URL to the output file with the resulting consensus.



consensus-url

_string_

Input/Output Ports

The element has 1 _input ports_:

**Name in GUI:** Input FASTA and VCF

**Name in Workflow File:** in-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Fasta url**

**fasta**

_string_

**VCF url**

**vcf**

_string_

And 1 _output port_:

**Name in GUI:** Fasta consensus URL

**Name in Workflow File:** out-consensus

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**out-consensus**

**out-consensus**

_string_
