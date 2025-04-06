---
title: "Searching Sequence Using HMM2 Profile"
weight: 1
---


# Searching Sequence Using HMM2 Profile

The _HMM search_ tool reads a HMM profile from a file and searches the sequence for significantly similar sequence matches.

The sequence must be selected in the _Project View_ or there must be an active _Sequence View_ window opened.

If the selected sequence is nucleic and the HMM profile is built for amino alignment, the sequence is automatically translated and all 6 translations are used to search in.

If a HMM profile is built for nucleic alignment, the search is performed for both strands (direct and complement).


![](/images/65930814/65930815.png)

The search results are stored as sequence annotations in the Genbank file format.


![](/images/65930814/65930816.png)

All HMM2 UGENE tools work only with files that contain a single HMM model.
