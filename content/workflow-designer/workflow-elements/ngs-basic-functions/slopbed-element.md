---
title: "Slopbed Element"
weight: 1
---


# Slopbed Element

Increases the size of each feature in files using bedtools slop.

**Element type:** slopbed

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

_numeric_

**Custom directory**

Specify the output directory.



**custom-dir**

_string_

**Output file name**

A name of an output file. If default of empty value is provided the output name is the name of the first file with additional extention.



**out-name**

_string_

**Genome**

In order to prevent the extension of intervals beyond chromosome boundaries, bedtools slop requires a genome file defining the length of each chromosome or contig (-g).

human.hg18

**genome-id**

_string_

**Each direction increase**

Increase the BED/GFF/VCF entry by the same number base pairs in each direction. If this parameter is used -l and -l are ignored. Enter 0 to disable (-b).

0

**b-id**

_numeric_

**Substract from start**

The number of base pairs to subtract from the start coordinate. Enter 0 to disable (-l).

0

**l-id**

_numeric_

**Add to end**

The number of base pairs to add to the end coordinate. Enter 0 to disable (-r).

0

**r-id**

_numeric_

**Strand-based**

Define -l and -r based on strand. For example. if used, -l 500 for a negative-stranded feature, it will add 500 bp to the end coordinate (-s).

False

**s-id**

_boolean_

**As fraction**

Define -l and -r as a fraction of the featureâs length. E.g. if used on a 1000bp feature, -l 0.50, will add 500 bp âupstreamâ (-pct).

False

**pct-id**

_boolean_

**Print header**

Print the header from the input file prior to results (-header).

False

**header-id**

_boolean_

Input/Output Ports

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
