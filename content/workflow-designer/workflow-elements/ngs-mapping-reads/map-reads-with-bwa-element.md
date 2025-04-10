---
title: "Map Reads with BWA Element"
weight: 400
---

# Map Reads with BWA Element

Performs alignment of short reads with BWA.

**Element type:** align-reads-with-bwa

| Parameter                   | Description                                       | Default Value | Parameter in Workflow File | Type     |
|-----------------------------|---------------------------------------------------|---------------|-----------------------------|----------|
| **Output directory**        | Directory to save BWA-MEM output files.           |               | **output-dir**              | _string_ |
| **Reference genome**        | Path to an indexed reference genome.              |               | **reference**               | _string_ |
| **Output file name**        | Base name of the output file. 'out.sam' by default.| out.sam       | **outname**                 | _string_ |
| **Library**                 | Is this library mate-paired?                      | single-end    | **library**                 | _string_ |
| **Use missing prob**        | Use missing probability instead of maximum edit distance.| True         | **use-miss-prob**           | _boolean_|
| **Missing prob**            | Missing probability (-n).                         | 0.04          | **missing-prob**            | _numeric_|
| **Seed length**             | Seed length (-l).                                 | 32            | **seed-length**             | _numeric_|
| **Max gap opens**           | Max gap opens (-o).                               | 1             | **max-gap**                 | _numeric_|
| **Index algorithm**         | Index algorithm (-a).                             | is            | **index-alg**               | _string_ |
| **Best hits**               | Best hits (-R).                                   | 30            | **best-hits**               | _numeric_|
| **Long-scaled gap penalty for long deletions** | Long-scaled gap penalty for long deletions (-L). | False       | **scaled-gap**              | _boolean_|
| **Non iterative mode**      | Non iterative mode (-N).                          | False         | **non-iterative**           | _boolean_|
| **Enable long gaps**        | Enable long gaps.                                 | True          | **enable-long-gaps**        | _boolean_|
| **Max gap extensions**      | Max gap extensions (-e).                          | 0             | **gap-extensions**          | _numeric_|
| **Indel offset**            | Indel offset (-i).                                | 5             | **indel-offset**            | _numeric_|
| **Max long deletions extensions** | Max long deletions extensions(-d).           | 10            | **long-deletions**          | _numeric_|
| **Barcode length**          | Barcode length (-B).                              | 0             | **barcode-length**          | _numeric_|
| **Max queue entries**       | Max queue entries (-m).                           | 2000000       | **max-queue**               | _numeric_|
| **Threads**                 | Threads (-t).                                     | 4             | **num-threads**             | _numeric_|
| **Max seed differences**    | Max seed differences (-k).                        | 2             | **max-seed**                | _numeric_|
| **Mismatch penalty**        | Mismatch penalty (-M).                            | 3             | **mistmatch-penalty**       | _numeric_|
| **Gap open penalty**        | Gap open penalty (-O).                            | 11            | **gap-open-penalty**        | _numeric_|
| **Gap extension penalty**   | Gap extension penalty; a gap of size k cost (-E). | 4             | **gap-ext-penalty**         | _numeric_|
| **Quality threshold**       | Quality threshold (-q).                           | 0             | **quality-threshold**       | _numeric_|

Input/Output Ports:

The element has 1 _input port_:

**Name in GUI:** BWA data

**Name in Workflow File:** in-data

| Slot In GUI                          | Slot in Workflow File | Type     |
|--------------------------------------|-----------------------|----------|
| **URL of a file with mate reads**    | **readsurl**          | _string_ |
| **URL of a file with reads**         | **readspairedurl**    | _string_ |

And 1 _output port_:

**Name in GUI:** BWA output data

**Name in Workflow File:** out-data

| Slot In GUI      | Slot in Workflow File | Type     |
|------------------|-----------------------|----------|
| **Assembly URL** | **assembly-out**      | _string_ |