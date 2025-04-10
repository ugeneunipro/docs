---
title: "Aligning with ClustalW"
weight: 1400
---

# Aligning with ClustalW

**Task Name:** align-clustalw

Multiple sequence alignment with ClustalW.

ClustalW is used as an [_external tool_](http://ugene.unipro.ru/documentation/manual/plugins/external_tool_support.html#external-tool-support) and must be installed on your system.

**Parameters:**

- _toolpath_ — path to the ClustalW executable. By default, the path specified in the _Application Settings_ is applied. \[String, Optional, Default: “default”\]

- _tmpdir_ — directory for temporary files. \[String, Optional\]

- _in_ — semicolon-separated list of input files. \[String, Required\]

- _out_ — output file. \[String, Required\]

- _format_ — format of the output file. \[String, Optional\]

**Example:**

`ugene align-clustalw --in=COI.aln --out=COI.sto --format=stockholm`