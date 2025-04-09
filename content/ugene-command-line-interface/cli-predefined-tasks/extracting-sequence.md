---
title: "Extracting Sequence"
weight: 300
---


# Extracting Sequence

**Task Name:** extract-sequence

Extracts annotated regions from an input sequence.

**Parameters:**

_in_ — semicolon-separated list of input files. \[String, Required\]

_out_ — output file. \[String, Required\]

_annotation-names_ — list of annotations names which will be accepted or filtered. \[String, Optional\]

_annotation-names-file -_ file with annotation names, separated with whitespaces which will be accepted or filtered. \[String, Optional\]

_accumulate - accumulate all incoming data in one file or create separate files for each input. In the latter case, an incremental numerical suffix is added to the file name (using 'True' by default). \[Boolean\]_

_accept-or-filter_ — if set to _true_, accepts only the specified annotations, if set to _false_, accepts all annotations except the specified ones. \[Boolean, Optional\]

_complement_ — complements the annotated regions if the corresponding annotation is located on the complement strand. \[Boolean, Optional\]

_extend-left_ — extends the resulting regions to the left for the specified number of base symbols. \[Number, Optional\]

_extend-right_ — extends the resulting regions to the right for the specified number of base symbols. \[Number, Optional\]

_gap-length_ — inserts a gap of the specified length between the merged annotations.

_transl_ - translates the annotated regions. \[Boolean, Optional\]

**Example:**

ugene extract-sequence --in=sars.gb --out=res.fa --annotation-names=gene
