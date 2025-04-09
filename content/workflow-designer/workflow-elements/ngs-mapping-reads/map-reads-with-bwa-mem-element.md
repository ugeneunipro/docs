---
title: "Map Reads with BWA-MEM Element"
weight: 500
---


# Map Reads with BWA-MEM Element

Performs alignment of short reads with BWA-MEM.

**Element type:** bwamem-id

Parameters

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Directory to save BWA-MEM output files.



**output-dir**

_string_

**Reference genome**

Path to an indexed reference genome.



**reference**

_string_

**Output file name**

Base name of the output file. 'out.sam' by default.

out.sam

**outname**

_string_

**Library**

Is this library mate-paired?

single-end

**library**

_string_

**Number of threads**

Number of threads (-t).

1

**threads**

_numeric_

**Min seed length**

Path to an indexed reference genome (-k).

19

**min-seed**

_numeric_

**Index algorithm**

Index algorithm (-a).

autodetect

**index-alg**

_string_

**Band width**

Bandwidth for banded alignment (-w).

100

**band-width**

_numeric_

**Dropoff**

Off-diagonal X-dropoff (-d).

100

**dropoff**

_numeric_

**Internal seed length**

Look for internal seeds inside a seed longer than {-k} (-r).

1.50000

**seed-lookup**

_numeric_

**Skip seed threshold**

Skip seeds with more than INT occurrences (-c).

10000

**seed-threshold**

_numeric_

**Drop chain threshold**

Drop chains shorter than FLOAT fraction of the longest overlapping chain (-D).

0.5

**drop-chains**

_numeric_

**Rounds of made rescues**

Perform at most INT rounds of mate rescues for each read (-m).

100

**mate-rescue**

_numeric_

**Skip mate rescue**

Skip mate rescue (-S).

False

**skip-mate-rescues**

_boolean_

**Skip pairing**

Skip pairing; mate rescue performed unless -S also in use (-P).

False

**skip-pairing**

_boolean_

**Matching score**

Score for a sequence match (-A).

1

**match-score**

_numeric_

**Mismatch penalty**

Penalty for a mismatch (-B).

4

**mistmatch-penalty**

_numeric_

**Gap open penalty**

Gap open penalty (-O).

6

**gap-open-penalty**

_numeric_

**Gap extension penalty**

Gap extension penalty; a gap of size k cost {-O} (-E).

1

**gap-ext-penalty**

_numeric_

**Penalty for clipping**

Penalty for clipping (-L).

5

**clipping-penalty**

_numeric_

**Penalty unpaired**

Penalty for an unpaired read pair (-U).

17

**inpaired-panalty**

_numeric_

**Score threshold**

Minimum score to output (-T).

30

 **score-threshold**

_numeric_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** BWA data

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

**Name in GUI:** BWA-MEM output data

**Name in Workflow File:** out-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Assembly URL**

**assembly-out**

_string_
