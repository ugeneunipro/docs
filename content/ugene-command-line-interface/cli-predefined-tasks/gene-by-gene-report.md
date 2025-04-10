---
title: "Gene-by-Gene Report"
weight: 2600
---

# Gene-by-Gene Report

**Task Name:** gene-by-gene

Suppose you have genomes and you want to characterize them. One way to do this is to build a table showing which genes are present in each genome and which are not.

1. Create a local BLAST database of your genome sequence/contigs. One database per genome.
2. Create a file with sequences of the genes you want to explore. This file will be the input file for the scheme.
3. Set up the location and name of the BLAST database you created for the first genome.
4. Set up output files: the report location and output file with annotated (via BLAST) sequences. You might want to delete the "Write Sequence" element if you do not need output sequences.
5. Run the scheme.
5*. Run the scheme on the same input and output files, changing the BLAST database for each genome that you have.

As a result, you will get a report file with "Yes" and "No" fields. A "Yes" indicates that the gene is present in the genome. A "No" might indicate that the gene is not present in the genome. It is a good idea to analyze all the "No" sequences using annotated files. Simply open a file and find a sequence with the name of a gene that has a "No" result.

**Parameters:**

- _in_: Input sequence file [URL datasets]
- _final-name_: Annotation name used to compare genes and reference genomes (using 'blast_result' by default) [String]
- _exist-file_: If a target report already exists, specify how to handle it. Merge two tables into one, overwrite, or rename the existing file (using 'Merge' by default) [String]
- _ident_: Identity between gene sequence length and annotation length in percent. BLAST identity (if specified) is checked after (using '90.0' percent by default) [Number]
- _out_: Output report file [String]
- _blast-out_: Location of BLAST output file [String]
- _search-type_: Type of BLAST searches (using 'blastn' by default) [String]
- _db-name_: Name of BLAST DB [String]
- _blast-path_: Path to BLAST DB [String]
- _expected-value_: This setting specifies the statistical significance threshold for reporting matches against database sequences (using '10.0' by default) [Number]
- _gapped-aln_: Perform gapped alignment (using 'use' by default) [Boolean]
- _blast-name_: Name for annotations (using 'blast_result' by default) [String]
- _tmpdir_: Directory for temporary files (using UGENE temporary directory by default) [String]
- _toolpath_: External tool path (using the path specified in UGENE by default) [String]
- _out-type_: Type of BLAST output file (using 'XML (-m 7)' by default) [String]

**Example:**

```sh
ugene gene-by-gene --in=human_T1.fa --out=human_T1_report