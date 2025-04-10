---
title: "Finding Repeats"
weight: 500
---

# Finding Repeats

**Task Name:** find-repeats

This task searches for repeats in sequences and saves the regions found as annotations.

**Parameters:**

- **_in_** — a semicolon-separated list of input files. \[String, Required\]
- **_out_** — the output file with the annotations. \[String, Required\]
- **_name_** — the name of the annotated regions. \[String, Optional, Default: “repeat\_unit”\]
- **_min-length_** — the minimum length of the repeats. \[Number, Optional, Default: 5\]
- **_identity_** — the percent identity between repeats. \[Number, Optional, Default: 100\]
- **_min-distance_** — the minimum distance between the repeats. \[Number, Optional, Default: 0\]
- **_max-distance_** — the maximum distance between the repeats. \[Number, Optional, Default: 5000\]
- **_inverted_** — if _true_, searches for the inverted repeats. \[Boolean, Optional, Default: false\]

**Example:**

```bash
ugene find-repeats --in=murine.gb --out=murine_repeats.gb --identity=99