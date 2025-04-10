---
title: "Reverse-Complement Converting Sequences"
weight: 2700
---

# Reverse-Complement Converting Sequences

**Task Name:** revcompl

Convert an input sequence into its reverse, complement, or reverse-complement counterpart and write the resulting sequence to a file.

**Parameters:**

- _type_ - Type of operation. Available options are 'Reverse Complement', 'Complement', and 'Reverse' ('Reverse Complement' is used by default) \[String\]

- _in_ - Input file \[URL datasets\]

- _accumulate_ - Accumulate all incoming data in one file or create separate files for each input. In the latter case, an incremental numerical suffix is added to the file name ('True' is used by default) \[Boolean\]

- _format_ - Output file format ('fasta' is used by default) \[String\]

- _split_ - Split each incoming sequence into several parts ('1' is used by default) \[Number\]

- _out_ - Output file \[String\]

**Example:**

ugene revcompl --in=human_T1.fa --out=human_T1_result.fa --format=fasta --type=reverse