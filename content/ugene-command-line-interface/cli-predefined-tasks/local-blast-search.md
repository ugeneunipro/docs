---
title: "Local BLAST Search"
weight: 1
---


# Local BLAST Search

**Task Name:** local-blast+

Performs a search on a local BLAST database using BLAST+.

BLAST+ is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

_toolpath_ — path to an appropriate BLAST executable (e.g. blastn, blastp, etc.). By default, the path specified in the _Application Settings_ is applied. \[String, Optional, Default: “default”\]

_tmpdir_ — directory for temporary files. By default, the path specified in the _Application Settings_ is applied. \[String, Optional, Default: “default”\]

_in_ — semicolon-separated list of input sequence files. \[String, Required\]

_dbpath_ — path to the BLAST database files. \[String, Required\]

_dbname_ — base name of the BLAST+ database files. \[String, Required\]

_out_ — output Genbank file, the results of the search are stored as annotations. \[String, Required\]

_name_ — name of the annotations. \[String, Optional, Default: “blast result”\]

_p_ — type of the BLAST search. \[String, Optional, Default: “blastn”\]

The following values are available:

*   *   blastn
    *   blastp
    *   blastx
    *   tblastn
    *   tblastx

_e_ — expectation value threshold. \[Number, Optional, Default: 10\]

**Example:**

ugene local-blast+ --in=input.fa --dbpath=. --dbname=mydb --out=output.gb
