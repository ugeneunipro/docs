---
title: "Map Reads with UGENE Genome Aligner Element"
weight: 600
---


# Map Reads with UGENE Genome Aligner Element

Unique UGENE algorithm for aligning short reads to reference genome.

**Element type:** genome-aligner

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output file name**

Base name of the output file. 'out.sam' by default.

out.sam

**outname**

 _string_

**Reference genome**

Path to an indexed reference genome.



**reference**

_string_

**Is absolute mismatches values?**

**true** \- absolute mismatches mode is used

**false** \- percentage mismatches mode is used

You can choose absolute or percentage mismatches values mode.

True

**if-absolute-mismatches-value**

_boolean_

**Absolute mismatches**

Number of mismatches allowed while aligning reads.

0

**absolute-mismatches**

_numeric_

**Align reverse complement reads**

Set this option to align both direct and reverse complement reads.

False

**reverse**

_boolean_

**Use "best"-mode**

Report only the best alignment for each read (in terms of mismatches).

True

**best**

_boolean_

**Omit reads with qualities lower than**

Omit reads with qualities lower than the specified value. Reads that have no qualities are not omitted.

Set "0" to switch off this option.

0

**quality-threshold**

_numeric_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Genome aligner data

**Name in Workflow File:** in-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**URL of a file with mate reads**

**readsurl**

_string_

**URL of a file with reads**

**readspairedurl**

_string_

And 1 _out__put port_:

**Name in GUI:** Genome aligner output data

**Name in Workflow File:** out-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Assembly URL**

**assembly-out**

_string_
