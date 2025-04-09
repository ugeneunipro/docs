---
title: "Aligning with MAFFT"
weight: 1700
---


# Aligning with MAFFT

**Task Name:** align-mafft

Multiple sequence alignment with MAFFT.

MAFFT is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

_toolpath_ — path to the MAFFT executable. By default, the path specified in the _Application Settings_ is applied. \[String, Optional, Default: “default”\]

_tmpdir_ — directory for temporary files. \[String, Optional\]

_in_ — semicolon-separated list of input files. \[String, Required\]

_out_ — output file. \[String, Required\]

_format_ — format of the output file. \[String, Required\]

_op_ — penalty for opening a gap. \[Number, Optional\]

_ep_ — penalty for extending a gap. \[Number, Optional\]

_maxiterate_ — maximum number of cycles of iterative refinement. \[Number, Optional\]

**Example:**

ugene align-mafft --in=COI.aln --out=COI\_aligned.aln
