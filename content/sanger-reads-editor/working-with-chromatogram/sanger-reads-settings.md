---
title: "Sanger Reads Settings"
weight: 900
---

# Sanger Reads Settings

Some mutations may have a chromatogram signal weaker than the reference one. This situation often arises when analyzing a mix of cells (healthy and oncological). This means that the mutation signal could vary due to the different concentration of oncological cells in a sample.

Look at the picture below. The signal of the "C" nucleotide (blue) is the highest. However, there is also a signal for the "T" nucleotide (red), which is significant. The second strongest signal is what we call an _Alternative mutation_.

![An Alternative mutation example](/images/66814020/66814029.png "An Alternative mutation example")

It is very important to make _Alternative mutations_ clearly visible. To accomplish this, you can use the function of the _Alternative mutation_. When this function is enabled and an _alternative mutation_ meets the settings, the corresponding character will be replaced with the alternative one. This replacement causes a difference between the read and the reference character, meaning the read character will be highlighted:

![A visible Alternative mutation](/images/66814020/66814043.png "A visible Alternative mutation")

The settings for _Alternative mutations_ are presented in the following picture:

![Settings of the function](/images/66814020/66814024.png "Settings of the function")

- _Show alternative mutations_ – Enable _Alternative mutations_ to display them if checked; otherwise, disable and hide them.
  
- _Threshold_ – Determines how strong the second strongest signal (relative to the first strongest signal) should be to be visible. In the picture below, the height of the second signal is 75% of the height of the first signal. This means the _threshold_ value should be set to 75% (or below) to make this _alternative mutation_ visible.

![](/images/66814020/66814051.png)

- _Update_ – Click this button to update the alignment according to the set values.