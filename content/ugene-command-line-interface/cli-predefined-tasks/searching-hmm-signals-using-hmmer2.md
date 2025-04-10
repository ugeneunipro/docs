---
title: "Searching HMM Signals Using HMMER2"
weight: 1200
---


# Searching HMM Signals Using HMMER2

**Task Name:** hmm2-search

This task searches each input sequence for significantly similar sequences that match all specified profile HMMs using the HMMER2 tool.

**Parameters:**

- _seq_: A semicolon-separated list of the input sequence files. \[String, Required\]

- _hmm_: A semicolon-separated list of the input HMM files. \[String, Required\]

- _out_: The output file with annotations. \[String, Required\]

- _name_: The name of the result annotations. \[String, Optional, Default: “hmm_signal”\]

- _e-val_: The e-value used to exclude low-probability hits from the result. \[Number, Optional, Default: 1e-1\]

- _score_: Score-based filtering, which is an alternative to e-value filtering, to exclude low-probability hits from the result. \[Number, Optional, Default: -1000000000\]

**Example:**

```
ugene hmm2-search --seq=CBS_seq.fa --hmm=CBS.hmm --out=CBS_hmm.gb