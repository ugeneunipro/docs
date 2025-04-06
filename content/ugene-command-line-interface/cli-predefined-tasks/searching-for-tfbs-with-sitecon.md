---
title: "Searching for TFBS with SITECON"
weight: 1
---


# Searching for TFBS with SITECON

**Task Name:** sitecon-search

Searches for transcription factor binding sites (TFBS) with SITECON and saves the regions found as annotations.

**Parameters:**

_in_ — semicolon-separated list of input sequence files to search TFBS in. \[String, Required\]

_inmodel_ — input SITECON profile(s). If several profiles have been supplied, searches with all profiles one by one and outputs merged set of annotations for each input sequence. \[String, Required\]

_out_ — output Genbank file. \[String, Required\]

_annotation-name_ — name of the annotated regions. \[String, Optional, Default: “misc\_feature”\]

_min-score_ — recognition quality threshold. The value must be between 60 and 100. Choosing too low threshold will lead to recognition of too many TFBS recognised with too low trustworthiness. Choosing too high threshold may result in no TFBS recognised. \[Number, Optional, Default: 85\]

_min-err1_ — setting for filtering results, minimal value of Error type I. \[Number, Optional, Default: 0\]

_max-err2_ — setting for filtering results, maximum value of Error type II. \[Number, Optional, Default: 0.001\]

_strand_ — strands to search in. \[Number, Optional, Default: 0\]

The following values are available:

*   *   0 (both strands)
    *   1 (direct strand)
    *   \-1 (complement strand)

**Example:**

ugene sitecon-search --in=input.fa --inmodel=profile.sitecon --out=res.gb
