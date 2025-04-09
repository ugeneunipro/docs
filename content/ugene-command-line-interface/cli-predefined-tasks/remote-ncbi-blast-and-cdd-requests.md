---
title: "Remote NCBI BLAST and CDD Requests"
weight: 900
---


# Remote NCBI BLAST and CDD Requests

**Task Name:** remote-request

Performs remote requests to the NCBI. Saves the results as annotations.

**Parameters:**

_in_ — semicolon-separated list of input files. A file can be of any format containing sequences or alignments. \[String, Required\]

_db_ — database to search in. \[String, Optional, Default: “ncbi-blastn”\]

The following databases are available:

*   *   “ncbi-blastn” for nucleotide sequences
    *   “ncbi-cdd” for amino acid sequences
    *   “ncbi-blastp” for amino acid sequences

_out_ — output Genbank file. \[String, Required\]

_eval_ — specifies the statistical significance threshold for reporting matches against database sequences. \[Number, Optional, Default: 10\]

_hits_ — maximum number of hits, that will be shown. \[Number, Optional, Default: 10\]

_name_ — name of the result annotations. If not set, name will be specified with the “cdd” result or the “blast” result. \[String, Optional, Default: “cdd” or “blast”\]

_short_ — optimizes search for short sequences. \[Boolean, Optional, Default: false\]

_blast-output_ — path to the file with the NCBI-BLAST output (only for the “ncbi-blastp” and “ncbi-blastn” databases). \[Boolean, Optional, Default: the file is not saved\]

**Example:**

ugene remote-request --in=seq.fa --db=ncbi-blastp --out=res.gb
