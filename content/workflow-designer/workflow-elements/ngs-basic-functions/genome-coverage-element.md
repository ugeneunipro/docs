---
title: "Genome Coverage Element"
weight: 900
---

# Genome Coverage Element

Calculates genome coverage using bedtools genomecov.

**Element type:** genomecov

| Parameter          | Description                                                                                                                                                          | Default value | Parameter in Workflow File | Type    |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|---------|
| **Output directory** | Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file. | Input file    |                            |         |
| **out-mode**       | _numeric_                                                                                                                                                            |               |                            |         |
| **Custom directory** | Specify the output directory.                                                                                                                                         |               | **custom-dir**             | _string_|
| **Output file name** | A name of an output file. If a default or empty value is provided the output name is the name of the first file with an additional extension.                         |               | **out-name**               | _string_|
| **Genome**         | To prevent the extension of intervals beyond chromosome boundaries, bedtools slop requires a genome file defining the length of each chromosome or contig (-g).        | human.hg18    | **genome**                 | _string_|
| **Report mode**    | Histogram - Compute a histogram of coverage.<br>Per-base (0-based) (-dz) - Compute the depth of feature coverage for each base on each chromosome (0-based).<br>Per-base (1-based) (-d) - Compute the depth of feature coverage for each base on each chromosome (1-based).<br>BEDGRAPH (-bg) - Produces genome-wide coverage output in BEDGRAPH format.<br>BEDGRAPH (including uncovered) (-bga) - Produces genome-wide coverage output in BEDGRAPH format (including uncovered). | Histogram     | **mode-id**                | _numeric_ |
| **Split**          | Treat "split" BAM or BED12 entries as distinct BED intervals when computing coverage. For BAM files, this uses the CIGAR "N" and "D" operations to infer the blocks for computing coverage. For BED12 files, this uses the BlockCount, BlockStarts, and BlockEnds fields (i.e., columns 10,11,12) (-split).      | False         | **split-id**               | _boolean_|
| **Strand**         | Calculate coverage of intervals from a specific strand. With BED files, requires at least 6 columns (strand is column 6) (-strand).                                    | False         | **strand-id**              | _boolean_|
| **5 prime**        | Calculate coverage of 5' positions (instead of the entire interval) (-5).                                                                                            | False         | **prime5-id**              | _boolean_|
| **3 prime**        | Calculate coverage of 3' positions (instead of the entire interval) (-3).                                                                                            | False         | **prime3-id**              | _boolean_|
| **Max**            | Combine all positions with a depth >= max into a single bin in the histogram (-max).                                                                                  | 2147483647    | **max-id**                 | _numeric_ |
| **Scale**          | Scale the coverage by a constant factor. Each coverage value is multiplied by this factor before being reported. Useful for normalizing coverage by, e.g., reads per million (RPM). Default is 1.0; i.e., unscaled (-scale). | 1.00000       | **scale-id**               | _numeric_ |
| **Trackline**      | Adds a UCSC/Genome-Browser track line definition in the first line of the output (-trackline).                                                                        | False         | **trackline-id**           | _boolean_|
| **Trackopts**      | Writes additional track line definition parameters in the first line (-trackopts).                                                                                      |               | **trackopts-id**           | _string_ |

Input/Output Ports

The element has 1 _input port_:

| Slot In GUI   | Slot in Workflow File | Type    |
|---------------|-----------------------|---------|
| **Name in GUI:** Input File | **Name in Workflow File:** in-file |         |
| **Source URL** | **url**               | _string_|

And 1 _output port_:

| Slot In GUI   | Slot in Workflow File | Type    |
|---------------|-----------------------|---------|
| **Name in GUI:** Output File | **Name in Workflow File:** out-file |         |
| **Source URL** | **url**               | _string_|