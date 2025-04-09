---
title: "Searching HMM Signals Using HMMER2"
weight: 1200
---


# Searching HMM Signals Using HMMER2

**Task Name:** hmm2-search

Searches each input sequence for the significantly similar sequence that matches to all specified profile HMM using the HMMER2 tool.

**Parameters:**

_seq_ — semicolon-separated list of the input sequence files. \[String, Required\]

_hmm_ — semicolon-separated list of the input HMM files. \[String, Required\]

_out_ — output file with annotations. \[String, Required\]

_name_ — name of the result annotations. \[String, Optional, Default: “hmm\_signal”\]

_e-val_ — e-value that can be used to exclude low-probability hits from the result. \[Number, Optional, Default: 1e-1\]

_score_ — score based filtering which is an alternative to e-value filtering to exclude low-probability hits from the result. \[Number, Optional, Default: -1000000000\]

**Example:**

ugene hmm2-search --seq=CBS\_seq.fa --hmm=CBS.hmm --out=CBS\_hmm.gb
