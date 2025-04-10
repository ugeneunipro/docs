---
title: "Aligning with MAFFT"
weight: 1700
---

# Aligning with MAFFT

**Task Name:** align-mafft

Perform multiple sequence alignment using MAFFT.

MAFFT is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

- _toolpath_ — The path to the MAFFT executable. By default, the path specified in the _Application Settings_ is used. \[String, Optional, Default: “default”\]

- _tmpdir_ — The directory for temporary files. \[String, Optional\]

- _in_ — A semicolon-separated list of input files. \[String, Required\]

- _out_ — The output file. \[String, Required\]

- _format_ — The format of the output file. \[String, Required\]

- _op_ — The penalty for opening a gap. \[Number, Optional\]

- _ep_ — The penalty for extending a gap. \[Number, Optional\]

- _maxiterate_ — The maximum number of cycles of iterative refinement. \[Number, Optional\]

**Example:**

```bash
ugene align-mafft --in=COI.aln --out=COI_aligned.aln