---
title: "DNA Generator"
weight: 400
---

# DNA Generator

The DNA sequence generator is a tool that generates a random DNA sequence with a specified nucleotide content. To generate a random DNA sequence, select the _Tools→Random sequence generator_ item in the main menu. The dialog will appear:

![](/images/65930704/65930705.png)

The following parameters are available:

- _Length_ - The length of the resulting sequence(s) (default is '1000' bp).

- _Window size_ - The DNA sequence generation is divided into windows of the specified size. In each window, the ratio of the base, defined by other parameters, is maintained (default is '1000').

- _Number of sequences_ - The number of sequences to generate (default is '1').

- _Initialize random generator manually_ - Value to initialize the random generator.

- _Reference_ - Path to the reference file (could be a sequence or an alignment).

- _Base content_ - Set the base content percentages manually.

- _GC Skew_ - Set the GC skew of the resulting sequence.

- _Output file_ - Output file.

- _Format_ - Output file format (default is 'fasta').

- _Add to project_ - Adds the generated sequence(s) to the project.

Once the _Generate_ button is pressed, the sequence(s) are created.