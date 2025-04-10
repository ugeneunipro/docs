---
title: "Building Statistical Profile for SITECON"
weight: 2300
---

# Building Statistical Profile for SITECON

**Task Name:** sitecon-build

Builds a statistical profile for SITECON, which can be used later to search for TFBS.

**Parameters:**

- **in** — A semicolon-separated list of input DNA multiple sequence alignment files. An input file should not contain gaps. \[String, Required\]

- **out** — Output file. If several input files have been supplied, then a sitecon profile is built for each input file. Thus, several output files (with different indexes) are generated. \[String, Required\]

- **wsize** — Window size. The window is a region of the alignment used to build the profile. It is selected from the center of the alignment and occupies the specified length. The edges of the alignment beyond the window are not considered. The recommended length is slightly less than the alignment length but not more than 50 bp. \[Number, Optional, Default: 40\]

- **clength** — Length of a random synthetic sequence used to calibrate the profile. \[Number, Optional, Default: 1000000\]

- **rseed** — Random seed used to calibrate the profile, for instance, to generate the random synthetic sequence. Use the same value to obtain the same calibration results on the same data. By default, a new random seed is generated each time a calibration occurs. \[Number, Optional, Default: 0\]

- **walg** — Specifies whether to use the _Algorithm 2_ weight algorithm. It is generally not required, but in some cases, it can enhance recognition quality. \[Boolean, Optional, Default: false\]

**Example:**

```
ugene sitecon-build --in=COI.aln --out=result.sitecon