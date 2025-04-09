---
title: "Map Reads with Bowtie Element"
weight: 200
---


# Map Reads with Bowtie Element

Performs alignment of short reads with Bowtie.

**Element type:** align-reads-with-bowtie

Parameters



**Output directory**

Directory to save Bowtie output files.



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

\-n mode

**mismatches\_type**

_string_

**Mismatches number**

Mismatches number.

2

**mismatches\_number**

_numeric_

**Mismatches number**

Maximum permitted total of quality values at all mismatched read positions throughout the entire alignment, not just in the seed. The default is 70. Like Maq, bowtie rounds quality values to the nearest 10 and saturates at 30; rounding can be disabled with --nomaqround.

70

**maqerr**

_numeric_

**Seed length**

The seed length; i.e., the number of bases on the high-quality end of the read to which the -n ceiling applies. The lowest permitted setting is 5 and the default is 28. bowtie is faster for larger values of -l.

28

**seedLen**

_numeric_

**Maximum of backtracks**

The maximum insert size for valid paired-end alignments. E.g. if -X 100 is specified and a paired-end alignment consists of two 20-bp alignments in the proper orientation with a 60-bp gap between them, that alignment is considered valid (as long as -I is also satisfied). A 61-bp gap would not be valid in that case. If trimming options -3 or -5 are also used, the -X constraint is applied with respect to the untrimmed mates, not the trimmed mates. Default: 250.

800

**maxbts**

_numeric_

**Best hits**

The number of megabytes of memory a given thread is given to store path descriptors in --best mode. Best-first search must keep track of many paths at once to ensure it is always extending the path with the lowest cumulative cost. Bowtie tries to minimize the memory impact of the descriptors, but they can still grow very large in some cases. If you receive an error message saying that chunk memory has been exhausted in --best mode, try adjusting this parameter up to dedicate more memory to the descriptors. Default: 64.

64

**chunkmbs**

_numeric_

**Seed**

Use as the seed for pseudo-random number generator.

0

**seed**

_numeric_

**Colorspace**

When -C is specified, read sequences are treated as colors. Colors may be encoded either as numbers (0=blue, 1=green, 2=orange, 3=red) or as characters A/C/G/T (A=blue, C=green, G=orange, T=red).

False

**colorspace**

_boolean_

**No Maq rounding**

Maq accepts quality values in the Phred quality scale, but internally rounds values to the nearest 10, with a maximum of 30. By default, bowtie also rounds this way. --nomaqround prevents this rounding in bowtie.

False

**nomaqround**

_boolean_

**No forward orientation**

If --nofw is specified, bowtie will not attempt to align against the forward reference strand.

False

**nofw**

_boolean_

**No reverse-complement orientation**

If --norc is specified, bowtie will not attempt to align against the reverse-complement reference strand.

False

**norc**

_boolean_

**Try as hard**

Try as hard as possible to find valid alignments when they exist, including paired-end alignments. This is equivalent to specifying very high values for the --maxbts and --pairtries options. This mode is generally much slower than the default settings, but can be useful for certain problems. This mode is slower when (a) the reference is very repetitive, (b) the reads are low quality, or (c) not many reads have valid alignments.

False

**tryhard**

_boolean_

**Best alignments**

Make Bowtie guarantee that reported singleton alignments are best in terms of stratum (i.e. number of mismatches, or mismatches in the seed in the case of -n mode) and in terms of the quality values at the mismatched position(s). bowtie is somewhat slower when --best is specified.

False

**best**

_boolean_

**All alignment**

Report all valid alignments per read or pair.

False

**all**

_boolean_

Parameter

Description

Default value

Parameter in Workflow File

Type

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Bowtie data

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

**Name in GUI:** Bowtie output data

**Name in Workflow File:** out-data

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Assembly URL**

**assembly-out**

_string_
