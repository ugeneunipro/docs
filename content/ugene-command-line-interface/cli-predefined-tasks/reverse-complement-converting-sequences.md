---
title: "Reverse-Complement Converting Sequences"
weight: 1
---


# Reverse-Complement Converting Sequences

**Task Name:** revcompl

Convert input sequence into its reverse, complement or reverse-complement counterpart and write result sequence to file

**Parameters:**

_type_ - Type of operation. Available are 'Reverse Complement', 'Complement' and 'Reverse' (using 'Reverse Complement' by default) \[String\]

 _in_ - Input file \[Url datasets\]

 _accumulate_ - Accumulate all incoming data in one file or create separate files for each input. In the latter case, an incremental numerical suffix is added to the file name (using 'True' by default) \[Boolean\]

 _format_ - Output file format (using 'fasta' by default) \[String\]

 _split_ - Split each incoming sequence on several parts (using '1' by default) \[Number\]

 _out_ - Output file \[String\]

**Example:**

ugene revcompl --in=human\_T1.fa --out=human\_T1\_result.fa --format=fasta --type=reverse
