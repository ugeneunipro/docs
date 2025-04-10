---
title: "Sanger Reads Consensus"
weight: 400
---

# Sanger Reads Consensus

Each base of a consensus sequence is calculated as a function of the corresponding column bases. The _Sanger Reads Editor_ allows switching between different consensus modes: Simple extended and Strict.

The Simple extended algorithm selects the best character from the extended DNA alphabet. Only bases with frequencies greater than a threshold value are taken into account.

The Strict algorithm returns a gap character ('-') if the symbol frequency in a column is lower than the specified threshold.

To switch the consensus mode, go to the _Consensus tab_ of the _Options Panel_:

![](/images/65929772/65929773.png)