---
title: "Finding Repeats"
weight: 500
---


# Finding Repeats

**Task Name:** find-repeats

Searches for repeats in sequences and saves the regions found as annotations.

**Parameters:**

_in_ — semicolon-separated list of input files. \[String, Required\]

_out_ — output file with the annotations. \[String, Required\]

_name_ — name of the annotated regions. \[String, Optional, Default: “repeat\_unit”\]

_min-length_ — minimum length of the repeats. \[Number, Optional, Default: 5\]

_identity_ — percent identity between repeats. \[Number, Optional, Default: 100\]

_min-distance_ — minimum distance between the repeats. \[Number, Optional, Default: 0\]

_max-distance_ — maximum distance between the repeats. \[Number, Optional, Default: 5000\]

_inverted_ — if _true_, searches for the inverted repeats. \[Boolean, Optional, Default: false\]

**Example:**

ugene find-repeats --in=murine.gb --out=murine\_repeats.gb --identity=99
