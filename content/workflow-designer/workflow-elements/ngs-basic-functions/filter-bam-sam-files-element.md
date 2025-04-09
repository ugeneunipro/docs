---
title: "Filter BAM SAM Files Element"
weight: 800
---


# Filter BAM SAM Files Element

Filters BAM/SAM files using SAMTools view.

**Element type:** filter-bam

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output folder**

Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.



**out-mode**

_numeric_

**Output name**

A name of an output BAM/SAM file. If the default of empty value is provided the output name is the name of the first BAM/SAM file with .filtered extension.



**out-name**

_string_

**Output format**

Format of an output assembly file.

bam

**out-format**

_string_

**Region**

Regions to filter. For BAM output only. chr2 to output the whole chr2. [chr2:1000](http://chr2:1000) to output regions of chr 2 starting from 1000. [chr2:1000-2000](http://chr2:1000-2000) to output regions of chr2 between 1000 and 2000 including the endpoint. To input, multiple regions use the space separator (e.g. chr1 chr2 [chr3:1000-2000](http://chr3:1000-2000)).



**region**

_string_

**MAPQ threshold**

Minimum MAPQ quality score.

0

**mapq**

_numeric_

**Accept flag**

Only output alignments with the selected items. Select the items in the combo box to configure the bit flag. Do not select the items to avoid filtration by this parameter.



**accept-flag**

_string_

**Skip flag**

Skip alignment with the selected items. Select the items in the combo box to configure the bit flag. Do not select the items to avoid filtration by this parameter.



**flag**

_string_



Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** BAM/SAM File

**Name in Workflow File:** in-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**input-url**

_string_

And 1 _out__put port_:

**Name in GUI:** Filtered BAM/SAM files

**Name in Workflow File:** out-file

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**output-url**

_string_
