---
title: "Assemble Transcripts with StringTie Element"
weight: 100
---

# Assemble Transcripts with StringTie Element

StringTie is a fast and highly efficient assembler of RNA-Seq alignments into potential transcripts. It uses a novel
network flow algorithm as well as an optional de novo assembly step to assemble and quantitate full-length transcripts
representing multiple splice variants for each gene locus.

**Element type:** stringtie

## Parameters

| Parameter                                  | Description                                                                                                                                                                                                                                                    | Default value | Parameter in Workflow File   | Type      |
|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------------|-----------|
| **Reference annotations**                  | Use the reference annotation file (in GTF or GFF3 format) to guide the assembly process (-G). The output will include expressed reference transcripts as well as any novel transcripts that are assembled.                                                     |               | **reference-annotations**    | _string_  |
| **Reads orientation**                      | Select the NGS libraries type: unstranded, stranded fr-secondstrand (--fr), or stranded fr-firststand (--rf).                                                                                                                                                  | Unstranded    | **reads-orientation**        | _string_  |
| **Label**                                  | Use the specified string as the prefix for the name of the output transcripts (-l).                                                                                                                                                                            | STRG          | **label**                    | _string_  |
| **Min isoform fraction**                   | Specify the minimum isoform abundance of the predicted transcripts as a fraction of the most abundant transcript assembled at a given locus (-f). Lower abundance transcripts are often artifacts of incompletely spliced precursors of processed transcripts. | 0.1           | **min-isoform-fraction**     | _numeric_ |
| **Min assembled transcript length**        | Specify the minimum length for the predicted transcripts (-m).                                                                                                                                                                                                 | 200           | **min-isoform-fraction**     | _numeric_ |
| **Min anchor length for junctions**        | Junctions that don't have spliced reads that align them with at least this amount of bases on both sides are filtered out (-a).                                                                                                                                | 10            | **min-anchor-length**        | _numeric_ |
| **Min junction coverage**                  | There should be at least this many spliced reads that align across a junction (-j). This number can be fractional since some reads align in more than one place. A read that aligns in n places will contribute 1/n to the junction coverage.                  | 1             | **min-junction-coverage**    | _numeric_ |
| **Trim transcripts based on coverage**     | By default StringTie adjusts the predicted transcript's start and/or stop coordinates based on sudden drops in coverage. Set to "False" to disable trimming (-t).                                                                                              | True          | **trim-transcripts**         | _bool_    |
| **Min coverage for assembled transcripts** | Specifies the minimum read coverage allowed for the predicted transcripts (-c). A transcript with lower coverage than this value is not shown in the output. This number can be fractional.                                                                    | 2.5           | **min-coverage**             | _numeric_ |
| **Min locus gap separation**               | Reads mapped closer than this distance are merged into the same processing bundle (-g).                                                                                                                                                                        | 50 bp         | **min-locus-gap**            | _numeric_ |
| **Fraction covered by multi-hit reads**    | Max fraction of multi-mapped reads allowed at a locus (-M). A read aligning in n places contributes 1/n to coverage.                                                                                                                                           | 0.95          | **multi-hit-fraction**       | _numeric_ |
| **Skip assembling for sequences**          | Ignore all read alignments for the specified reference sequences (-x). Useful for skipping mitochondrial genome, etc. Case sensitive.                                                                                                                          |               | **skip-sequences**           | _string_  |
| **Multi-mapping correction**               | Enables or disables multi-mapping correction (-u).                                                                                                                                                                                                             | Enabled       | **multi-mapping-correction** | _bool_    |
| **Verbose log**                            | Enable detailed logging (-v). Messages go to UGENE log and dashboard.                                                                                                                                                                                          | False         | **verbose-log**              | _bool_    |
| **Number of threads**                      | Number of processing threads to use (-p).                                                                                                                                                                                                                      | 8             | **threads**                  | _numeric_ |
| **Output transcripts file**                | Primary GTF output file with assembled transcripts.                                                                                                                                                                                                            | Auto          | **transcripts-output-url**   | _string_  |
| **Enable gene abundance output**           | Generate gene abundances file (-A). File URL is passed to an output slot.                                                                                                                                                                                      | False         | **gene-abundance-output**    | _bool_    |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Input BAM file(s)
**Name in Workflow File:** in
**Slots:**

| Slot in GUI    | Slot in Workflow File | Type     |
|----------------|-----------------------|----------|
| **Source URL** | url                   | _string_ |

And 1 _output port_:

**Name in GUI:** StringTie output data
**Name in Workflow File:** out
**Slots:**

| Slot in GUI    | Slot in Workflow File | Type     |
|----------------|-----------------------|----------|
| **Output URL** | url                   | _string_ |
