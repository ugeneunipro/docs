---
title: "Building Profile HMM Using HMMER2"
weight: 1
---


# Building Profile HMM Using HMMER2

**Task Name:** hmm2-build

Builds a profile HMM using the HMMER2 tools.

**Parameters:**

_in_ — semicolon-separated list of input multiple sequence alignment files. \[String, Required\]

_out_ — output HMM file. \[String, Required\]

_name_ — name of the profile HMM. \[String, Optional, Default: “hmm\_profile”\]

_calibrate_ — enables/disables calibration. \[Boolean, Optional, Default: true\]

_seed_ — random seed, a non-negative integer. \[Number, Optional, Default: 0\]

**Example:**

ugene hmm2-build --in=CBS.sto --out=CBS.hmm
