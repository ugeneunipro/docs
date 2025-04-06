---
title: "Generating DNA Sequence"
weight: 1
---


# Generating DNA Sequence

**Task Name:** generate-dna

Generates a random DNA sequence with specified nucleotide content

**Parameters:**

_algo_ - Algorithm for generating (using 'GC Content' by default) \[String\]

_content_ - Specifies if the nucleotide content of generated sequence(s) will be taken from reference or specified manually (A, G, C, T parameters) (using 'manual' by default) \[String\]

_count_ - Number of sequences to generate (using '1' by default) \[Number\]

_length_ - Length of the resulted sequence(s) (using '1000' bp by default) \[Number\]

_a_ - Adenine content (using '25' percents by default) \[Number\]

_c_ - Cytosine content (using '25' percents by default) \[Number\]

_g_ - Guanine content (using '25' percents by default) \[Number\]

_t_ - Thymine content (using '25' percents by default) \[Number\]

_ref_ - Path to the reference file (could be a sequence or an alignment) \[String\]

_seed_ - Value to initialize the random generator. By default (seed = -1) the generator is initialized with the system time (using '-1' by default) \[Number\]

_wnd-size_ - Size of window where set content (using '1000' by default) \[Number\]

_accumulate_ - Accumulate all incoming data in one file or create separate files for each input. In the latter case, an incremental numerical suffix is added to the file name (using 'True' by default) \[Boolean\]

_format_ - Output file format (using 'fasta' by default) \[String\]

_split_ - Split each incoming sequence on several parts (using '1' by default) \[Number\]

_out_ - Output file \[String\]

**Example:**

ugene generate-dna --length=2000 --a=45 --out=test.fa
