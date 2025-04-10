---
title: "Generating DNA Sequence"
weight: 2900
---

# Generating DNA Sequence

**Task Name:** generate-dna

Generates a random DNA sequence with specified nucleotide content.

**Parameters:**

- _algo_ - Algorithm for generation (default is 'GC Content') \[String\]

- _content_ - Specifies if the nucleotide content of the generated sequence(s) will be taken from a reference or specified manually (A, G, C, T parameters) (default is 'manual') \[String\]

- _count_ - Number of sequences to generate (default is '1') \[Number\]

- _length_ - Length of the resulting sequence(s) (default is '1000' bp) \[Number\]

- _a_ - Adenine content (default is '25%') \[Number\]

- _c_ - Cytosine content (default is '25%') \[Number\]

- _g_ - Guanine content (default is '25%') \[Number\]

- _t_ - Thymine content (default is '25%') \[Number\]

- _ref_ - Path to the reference file (can be a sequence or an alignment) \[String\]

- _seed_ - Value to initialize the random generator. By default (seed = -1), the generator is initialized with the system time (default is '-1') \[Number\]

- _wnd-size_ - Size of the window where content is set (default is '1000') \[Number\]

- _accumulate_ - Accumulate all incoming data in one file or create separate files for each input. In the latter case, an incremental numerical suffix is added to the file name (default is 'True') \[Boolean\]

- _format_ - Output file format (default is 'fasta') \[String\]

- _split_ - Split each incoming sequence into several parts (default is '1') \[Number\]

- _out_ - Output file \[String\]

**Example:**

`ugene generate-dna --length=2000 --a=45 --out=test.fa`