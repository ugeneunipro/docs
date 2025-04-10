---
title: "Annotating Sequence with UQL Schema"
weight: 1000
---

# Annotating Sequence with UQL Schema

**Task Name:** query

Annotates a sequence in compliance with a UGENE Query Language (UQL) schema. This allows the analysis of a sequence using different algorithms while imposing constraints on the positional relationship of the results.

To learn more about the UQL schemas, read the [Query Designer Manual](http://ugene.unipro.ru/documentation.html).

**Parameters:**

- _in_ — semicolon-separated list of input sequence files. \[String, Required\]
- _out_ — output Genbank file with the annotations. \[String, Required\]
- _schema_ — UQL schema. \[String, Required\]
- _merge_ — if true, merges regions of each result into a single annotation. \[Boolean, Optional, Default: false\]
- _offset_ — if _merge_ is set to true, specifies left and right offsets for merged annotations. \[Number, Optional, Default: 0\]

**Example:**

ugene query --in=input.fa --out=result.gb --schema=RepeatsWithORF.uql