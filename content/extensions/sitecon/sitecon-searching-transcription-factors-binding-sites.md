---
title: "SITECON Searching Transcription Factors Binding Sites"
weight: 100
---

# SITECON: Searching Transcription Factor Binding Sites

To search for transcription factor binding sites in a DNA sequence, select the _Analyze ‣ Search TFBS with SITECON..._ option from the context menu.

In the search dialog that appears, you must select a file with a TFBS profile. The profiles supplied with UGENE are located in the $UGENE/data/sitecon_models folder.

Once the profile is loaded, the threshold filter is populated with values read from the profile. You can use the filter to remove low-scoring regions from the results.

![](/images/65930797/65930798.png)

The regions found by the SITECON algorithm can be saved as annotations to the DNA sequence in Genbank format.

Every _SITECON_ profile supplied with UGENE contains complete information about calibration settings provided to the UGENE team by the author of _SITECON_.

The original TFBS alignments used to calculate profiles can be requested directly from the author of _SITECON_.