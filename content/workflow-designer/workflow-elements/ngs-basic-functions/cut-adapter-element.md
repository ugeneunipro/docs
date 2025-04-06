---
title: "Cut Adapter Element"
weight: 1
---


# Cut Adapter Element

Removes adapter sequences.

**Element type:** CutAdaptFastq

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.

Input file

**out-mode**

_string_

**Output file name**

A name of an output file. If default of empty value is provided the output name is the name of the first file with additional extention.



**out-name**

_string_

**FASTA file with 3' adapters**

A FASTA file with one or multiple sequences of adapter that were ligated to the 3' end. The adapter itself and anything that follows is trimmed. If the adapter sequence ends with the '$ character, the adapter is anchored to the end of the read and only found if it is a suffix of the read.



**adapters-url**

_string_

**FASTA file with 5' adapters**

A FASTA file with one or multiple sequences of adapters that were ligated to the 5' end. If the adapter sequence starts with the character '^', the adapter is 'anchored'. An anchored adapter must appear in its entirety at the 5' end of the read (it is a prefix of the read). A non-anchored adapter may appear partially at the 5' end, or it may occur within the read. If it is found within a read, the sequence preceding the adapter is also trimmed. In all cases, the adapter itself is trimmed.



**front-url**

_string_

**FASTA file with 5' and 3' adapters**

A FASTA file with one or multiple sequences of adapters that were ligated to the 5' end or 3' end.



**anywhere-url**

_string_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input File

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_

And 1 _output port_:

**Name in GUI:** Output File

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**url**

_string_
