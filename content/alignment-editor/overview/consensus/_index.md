---
title: "Consensus"
weight: 700
---

# Consensus

Each base of a consensus sequence is calculated as a function of the corresponding column bases (and, for some algorithms, the column bases of the whole alignment). There are different methods to calculate the consensus, and each method reveals unique biological properties of the aligned sequences. The _Alignment Editor_ allows switching between different consensus modes. To switch the consensus mode, go to the _General tab_ of the _Options Panel_, activate the context menu (using the right mouse button), or use the _Actions_ menu and select the _Consensus mode_ item. The _General tab_ will open automatically:

![](/images/65929634/65929635.png)

There are several consensus modes:

* **Default** — The mode is based on the JalView algorithm. A character in the consensus is calculated based on the characters in the corresponding column and the value of the threshold:
  * If the percentage value of the most frequent character is greater than the threshold, the character is shown in uppercase in the consensus.
  * If there are two characters with the equal highest frequency in a column, the '+' sign is shown.
  * If the percentage value of the most frequent character is high but lower than the specified threshold, the character is shown in lowercase in the consensus.
  
* **ClustalW** — Emulates the ClustalW program behavior.
  * If the percentage value of the most frequent character is equal to 100%, the '**\***' base is shown in the consensus.
  * Otherwise, no characters are shown.
  
* **Levitsky** (not for AMINO alignment) — Proposed by Victor Levitsky, this mode calculates the consensus of a DNA alignment, taking into account the frequencies of characters in the whole alignment, not just one column. The algorithm includes these steps:
  1. Collect global alignment frequencies for every character in alignment using the [extended DNA alphabet](https://en.wikipedia.org/wiki/Nucleic_acid_notation). For example, the **A** base increments the counter of the following bases:
      * A (the base itself),
      * W (A or T),
      * R (A or G),
      * M (A or C),
      * V (A or C or G),
      * H (A or C or T),
      * D (A or G or T),
      * N (A or C or G or T).
  2. Check the frequency of each symbol in the column:
      * If the frequency percentage value is greater than the threshold, this base is considered a consensus symbol - see further algorithm description.
      * If the frequency percentage value is lower than the specified threshold, this base is **not** considered a consensus symbol.
  3. From the set of bases not filtered in point **2**, choose the rarest characters in the whole alignment (global frequencies have been calculated in point **1**):
      * If there is only one base, this character is shown in the consensus.
      * If there are two or more bases, these symbols should be joined into one common base. For example, if there are two bases **A** and **T**, they will be joined into an extended DNA alphabet base **W**. Check [this](https://en.wikipedia.org/wiki/Nucleic_acid_notation#IUPAC_notation) table for all possible combinations.
      
* **Simple extended** (not for AMINO alignment) — A character of the consensus is calculated based on the characters in the corresponding column. This algorithm joins all bases in the column (but only those with a frequency percentage value greater than the threshold) into a single base from the DNA extended alphabet using [this](https://en.wikipedia.org/wiki/Nucleic_acid_notation#IUPAC_notation) table.
  
* **Strict** — If a character's percentage in a column is higher than the specified threshold, the character is shown in the consensus at this position. Otherwise, a gap character (‘—’) is shown.

Also, the _General tab_ shows general information about an alignment and allows one to set up a reference sequence. The following chapter describes how to export a consensus sequence: