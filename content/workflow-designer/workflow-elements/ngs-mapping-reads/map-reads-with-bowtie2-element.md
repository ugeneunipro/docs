---
title: "Map Reads with Bowtie2 Element"
weight: 1
---


# Map Reads with Bowtie2 Element

Performs alignment of short reads with Bowtie2.

**Element type:** align-reads-with-bowtie2

Parameters in GUI

**Output directory**

Directory to save Bowtie2 output files.



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

**Mode**

When the -n option is specified (which is the default), bowtie determines which alignments are valid according to the following policy, which is similar to Maq's default policy. In -v mode, alignments may have no more than V mismatches, where V may be a number from 0 through 3 set using the -v option. Quality values are ignored. The -v option is mutually exclusive with the -n option.

\--end-to-end

**mode**

_string_

**Number of mismatches**

Sets the number of mismatches to allowed in a seed alignment. Can be set to 0 or 1. Setting this higher makes alignment slower (often much slower) but increases sensitivity.

0

**mismatches\_number**

_numeric_

**Seed length (--L)**

Sets the length of the seed substrings to align. Smaller values make alignment slower but more senstive.

20

**seed\_len**

_numeric_

**Add columns to allow gaps (--dpad)**

"Pads" dynamic programming problems by the specified number of columns on either side to allow gaps.

15

**dpad**

_numeric_

**Disallow gaps (--gbar)**

Disallow gaps within a specified number of positions of the beginning or end of the read.

4

**gbar**

_numeric_

**Seed (--seed)**

Use as the seed for pseudo-random number generator.

0

**seed**

_numeric_

**Threads**

Launch specified number of parallel search threads. Threads will run on separate processors/cores and synchronize when parsing reads and outputting alignments. Searching for alignments is highly parallel, and speedup is close to linear.

1

**threads**

_numeric_

**No unpaired alignments (--no-mixed)**

If Bowtie2 cannot find a paired-end alignment for a pair, by default it will go on to look for unpaired alignments for the constituent mates. This is called "mixed mode." To disable mixed mode, set this option. Bowtie2 runs a little faster in the mixed mode, but will only consider the alignment status of pairs per se, not individual mates.

False

**nomixed**

_boolean_

**No discordant alignments (--no-discordant)**

By default, Bowtie2 looks for discordant alignments if it cannot find any concordant alignments. A discordant alignment is an alignment where both mates align uniquely, but that does not satisfy the paired-end constraints. This option disables that behavior.

False

**nodiscordant**

_boolean_

**No forward orientation (--nofw)**

If --nofw is specified, bowtie will not attempt to align against the forward reference strand.

False

**nofw**

_boolean_

**No reverse-complement orientation (--norc)**

If --norc is specified, bowtie will not attempt to align against the reverse-complement reference strand.

False

**norc**

_boolean_

**No overlapping mates (--no-overlap)**

If one mate alignment overlaps the other at all, consider that to be non-concordant. Default: mates can overlap in a concordant alignment.

False

**nooverlap**

_boolean_

**No mates containing one another (--no-contain)**

If one mate alignment contains the other, consider that to be non-concordant. Default: a mate can contain the other in a concordant alignment.

False

**nocontain**

_boolean_

Parameter

Description

Default value

Parameter in Workflow File

Type

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Bowtie2 data

**Name in Workflow File:** in-data

**Slots:**

**URL of a file with mate reads**

**readsurl**

_string_

**URL of a file with reads**

**readspairedurl**

_string_

Slot In GUI

Slot in Workflow File

Type

And 1 _out__put port_:

**Name in GUI:** Bowtie2 output data

**Name in Workflow File:** out-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Assembly URL**

**assembly-out**

_string_
