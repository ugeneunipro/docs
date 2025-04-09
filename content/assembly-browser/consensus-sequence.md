---
title: "Consensus Sequence"
weight: 700
---


# Consensus Sequence

A consensus sequence can be found in the _Consensus Area_ under a reference sequence. It refers to the most common nucleotide at a particular position.


![](/images/65929837/65929838.png)

To choose a consensus algorithm select the _Consensus algorihtm_ item either in the context menu of the _Consensus Area_, in the context menu of the _Reads Area_ or on the _Assembly Browser Settings_ tab of the _Options Panel_. .

The following algorithms are currently available:

*   _Default_ — shows the most common nucleotide at each position. When there is equal numbers of different nucleotides in a position, the consensus sequence resulting nucleotide is selected randomly from these nucleotides.
*   _SAMtools_ — uses an algorithm from the SAMtools Text Alignment Viewer to build the consensus sequence. The algorithm takes into account quality values of reads and nucleotides and works with the extended nucleotide alphabet.

To leave only differences between the reference and the consensus sequences highlighted on the consensus sequence, select the _Show difference from reference_ item in the context menu of the _Consensus Area_ or the _Difference from reference_ item on the _Assembly Browser Settings_tab of the _Options Panel_:


![](/images/65929837/65929839.png)

To export a _Consensus Sequence_, right-click on it in the _Consensus Area_ and select the _Export ‣ Export consensus_ item in the context menu. For more information about consensus exporting see [_Exporting Consensus_](exporting/exporting-consensus).
