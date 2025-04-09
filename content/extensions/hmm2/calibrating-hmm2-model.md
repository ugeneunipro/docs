---
title: "Calibrating HMM2 Model"
weight: 200
---


# Calibrating HMM2 Model

The _HMM calibrate_ tool reads a HMM profile file, scores a large number of synthesized random sequences with it, fits an extreme value distribution (EVD) to the histogram of those scores, and re-saves the hmm file including the EVD parameters.

To avoid modification of the original HMM file you can select a new location for the calibrated profile.


![](/images/65930812/65930813.png)
