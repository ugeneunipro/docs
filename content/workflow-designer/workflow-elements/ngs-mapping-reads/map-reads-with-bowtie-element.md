---
title: "Map Reads with Bowtie Element"
weight: 200
---

# Map Reads with Bowtie Element

This page provides information on performing alignment of short reads using Bowtie.

**Element type:** align-reads-with-bowtie

Parameters

| Parameter                                | Description                                                                                                                                                                                                                                                                                                | Default value | Type    |
|------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|---------|
| **Output directory**                     | Directory to save Bowtie output files.                                                                                                                                                                                                                                                                    |               | _string_|
| **output-dir**                           | Directory path for saving output files.                                                                                                                                                                                                                                                                     |               | _string_|
| **Reference genome**                     | Path to an indexed reference genome.                                                                                                                                                                                                                                                                      |               | _string_|
| **reference**                            | Path location of the reference genome.                                                                                                                                                                                                                                                                    |               | _string_|
| **Output file name**                     | Base name of the output file. By default, it is 'out.sam'.                                                                                                                                                                                                                                                | out.sam       | _string_|
| **Library**                              | Specifies if the library is mate-paired.                                                                                                                                                                                                                                                                  | single-end    | _string_|
| **Mode**                                 | Determines the valid alignments policy. In -v mode, alignments may have no more than V mismatches, where V is a number from 0 through 3. Quality values are ignored. The -v option is mutually exclusive with the -n option.                                                                                   | -n mode       | _string_|
| **mismatches_type**                      | Alignment policy type according to the mismatches.                                                                                                                                                                                                                                                        | -n mode       | _string_|
| **Mismatches number**                    | Number of mismatches allowed.                                                                                                                                                                                                                                                                              | 2             | _numeric_|
| **maqerr**                               | Maximum permitted sum of quality values at mismatched read positions throughout the alignment. Default is 70.                                                                                                                                                                                             | 70            | _numeric_|
| **Seed length**                          | Number of bases on the high-quality end of the read for the -n ceiling to apply. Faster for larger values.                                                                                                                                                                                                | 28            | _numeric_|
| **seedLen**                              | Length of the seed.                                                                                                                                                                                                                                                                                       | 28            | _numeric_|
| **Maximum of backtracks**                | Maximum insert size for valid paired-end alignments. With a default of 250.                                                                                                                                                                                                                               | 800           | _numeric_|
| **maxbts**                               | Maximum backtrack setting.                                                                                                                                                                                                                                                                                | 800           | _numeric_|
| **Best hits**                            | Amount of memory in megabytes provided to store path descriptors in --best mode. Default is 64.                                                                                                                                                                                                           | 64            | _numeric_|
| **chunkmbs**                             | Memory allocation for best hits.                                                                                                                                                                                                                                                                          | 64            | _numeric_|
| **Seed**                                 | Seed for pseudo-random number generator.                                                                                                                                                                                                                                                                  | 0             | _numeric_|
| **Colorspace**                           | When -C is specified, read sequences are treated as colors.                                                                                                                                                                                                                                               | False         | _boolean_|
| **No Maq rounding**                      | Disables rounding of quality values in the Phred quality scale.                                                                                                                                                                                                                                           | False         | _boolean_|
| **No forward orientation**               | Prevents alignment against the forward reference strand.                                                                                                                                                                                                                                                  | False         | _boolean_|
| **No reverse-complement orientation**    | Prevents alignment against the reverse-complement reference strand.                                                                                                                                                                                                                                       | False         | _boolean_|
| **Try as hard**                          | Attempts to find all valid alignments, including paired-end alignments. Useful but slower than default.                                                                                                                                                                                                   | False         | _boolean_|
| **Best alignments**                      | Guarantees reported singleton alignments are best in terms of mismatches and quality values. Slower operation when specified.                                                                                                                                                                              | False         | _boolean_|
| **All alignment**                        | Reports all valid alignments per read or pair.                                                                                                                                                                                                                                                            | False         | _boolean_|

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Bowtie data

**Name in Workflow File:** in-data

**Slots:**

| Slot In GUI                        | Slot in Workflow File | Type    |
|------------------------------------|-----------------------|---------|
| **URL of a file with mate reads**  | **readsurl**          | _string_|
| **URL of a file with reads**       | **readspairedurl**    | _string_|

And 1 _output port_:

**Name in GUI:** Bowtie output data

**Name in Workflow File:** out-data

**Slots:**

| Slot In GUI      | Slot in Workflow File | Type    |
|------------------|-----------------------|---------|
| **Assembly URL** | **assembly-out**      | _string_|