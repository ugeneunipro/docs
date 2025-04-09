---
title: "Assembly Sequences with CAP3"
weight: 100
---

# Assembly Sequences with CAP3

CAP3 is a contig assembly program. It allows assembly long DNA reads (up to 1000 bp).

Binaries can be downloaded from [http://seq.cs.iastate.edu/cap3.html](http://seq.cs.iastate.edu/cap3.html)
Huang, X. and Madan, A. (1999) CAP3: A DNA Sequence Assembly Program, Genome Research, 9: 868-877.

**Element type:** cap3

## Parameters

| Parameter                           | Description                                                                                                                           | Default value | Parameter in Workflow File   | Type      |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------------|-----------|
| **Output file**                     | Write assembly results to this output file in ACE format.                                                                             | result.ace    | **out-file**                 | _string_  |
| **Quality cutoff for clipping**     | Base quality cutoff for clipping (-c).                                                                                                | 12            | **clipping-cutoff**          | _numeric_ |
| **Clipping range**                  | Set a number which unit is base. It will get the refGenes in n bases from peak center. (--distance).                                  | 100           | **clipping-range**           | _numeric_ |
| **Quality cutoff for differences**  | Base quality cutoff for differences (-b).                                                                                             | 20            | **diff-cutoff**              | _numeric_ |
| **Maximum difference score**        | Max qscore sum at differences (-d). If an overlap contains lots of differences at bases of high quality, then the overlap is removed. | 200           | **diff-max-qscore**          | _numeric_ |
| **Match score factor**              | Affects similarity score of an overlap (-m).                                                                                          | 2             | **match-score-factor**       | _numeric_ |
| **Mismatch score factor**           | Affects similarity score of an overlap (-n).                                                                                          | -5            | **mismatch-score-factor**    | _numeric_ |
| **Gap penalty factor**              | Affects similarity score of an overlap (-g).                                                                                          | 6             | **gap-penalty-factor**       | _numeric_ |
| **Overlap similarity score cutoff** | If the similarity score of an overlap is less than this cutoff (-s), the overlap is removed.                                          | 900           | **overlap-sim-score-cutoff** | _numeric_ |
| **Overlap length cutoff**           | Overlaps must be at least this long in bp (-o).                                                                                       | 40            | **overlap-length-cutoff**    | _numeric_ |
| **Overlap percent identity cutoff** | Overlaps must meet or exceed this percent identity (-p).                                                                              | 90            | **overlap-perc-id-cutoff**   | _numeric_ |
| **Max number of word matches**      | Upper limit for the number of word matches considered (-t). Controls tradeoff between accuracy and speed.                             | 300           | **max-num-word-matches**     | _numeric_ |
| **Band expansion size**             | CAP3 expands alignment bands by this size (-a).                                                                                       | 20            | **band-exp-size**            | _numeric_ |
| **Max gap length in an overlap**    | Maximum length of gap in overlaps allowed (-f).                                                                                       | 20            | **max-gap-in-overlap**       | _numeric_ |
| **Assembly reverse reads**          | Whether to consider reverse orientation reads in assembly (-r).                                                                       | True          | **assembly-reverse**         | _boolean_ |
| **CAP3 tool path**                  | Path to the CAP3 executable.                                                                                                          | default       | **path**                     | _string_  |
| **Temporary directory**             | Directory for temporary files.                                                                                                        | default       | **tmp-dir**                  | _string_  |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Input sequences
**Name in Workflow File:** in-data
**Slots:**

| Slot In GUI      | Slot in Workflow File | Type     |
|------------------|-----------------------|----------|
| **Dataset name** | **dataset**           | _string_ |
| **Input URL(s)** | **in.url**            | _string_ |
