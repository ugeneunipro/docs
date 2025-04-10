---
title: "Searching for TFBS with SITECON"
weight: 2400
---

# Searching for TFBS with SITECON

**Task Name:** sitecon-search

The tool searches for transcription factor binding sites (TFBS) using SITECON and saves the identified regions as annotations.

**Parameters:**

- _in_ — A semicolon-separated list of input sequence files to search for TFBS. \[String, Required\]
  
- _inmodel_ — Input SITECON profile(s). If several profiles are supplied, the tool searches using all profiles one by one and outputs a merged set of annotations for each input sequence. \[String, Required\]
  
- _out_ — Output Genbank file. \[String, Required\]
  
- _annotation-name_ — Name of the annotated regions. \[String, Optional, Default: “misc_feature”\]
  
- _min-score_ — Recognition quality threshold. The value must be between 60 and 100. Choosing a threshold too low will result in recognizing too many TFBS with low reliability, while choosing it too high may result in no TFBS being recognized. \[Number, Optional, Default: 85\]
  
- _min-err1_ — Setting for filtering results, minimum value of Error type I. \[Number, Optional, Default: 0\]
  
- _max-err2_ — Setting for filtering results, maximum value of Error type II. \[Number, Optional, Default: 0.001\]
  
- _strand_ — Strands to search in. \[Number, Optional, Default: 0\]

  The following values are available:

  * 0 (both strands)
  * 1 (direct strand)
  * -1 (complement strand)

**Example:**

```
ugene sitecon-search --in=input.fa --inmodel=profile.sitecon --out=res.gb