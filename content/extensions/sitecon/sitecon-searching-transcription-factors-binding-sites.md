---
title: "SITECON Searching Transcription Factors Binding Sites"
weight: 1
---


# SITECON Searching Transcription Factors Binding Sites

To search transcription factor binding sites in a DNA sequence select the _Analyze ‣ Search TFBS with SITECON..._ context menu item.

In the appeared search dialog you must select a file with TFBS profile. The profiles supplied with UGENE are placed in the $UGENE/data/sitecon\_models folder.

After the profile is loaded the threshold-filter is populated with values read from profile. You can use the filter to remove low-scoring regions from the result.


![](/images/65930797/65930798.png)

The regions found by SITECON algorithm can be saved as annotations to the DNA sequence in the Genbank format.

Every _SITECON_ profile supplied with UGENE contains complete information about calibration settings provided to UGENE team by the author of _SITECON_.

The original TFBS alignments used to calculate profiles can be requested directly from the author of _SITECON_.
