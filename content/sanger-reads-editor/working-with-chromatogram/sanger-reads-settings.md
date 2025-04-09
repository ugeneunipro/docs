---
title: "Sanger Reads Settings"
weight: 900
---


# Sanger Reads Settings

Some mutations could have a chromatogram signal lesser than the reference one. This situation very often appears if the mix of cells (healthy and oncological) has been being analyzed. That means that the mutation signal could be different (due to a different concentration of oncological cells in a sample).

Look at the picture below. The signal of the "C" nucleotide (blue) is the highest. But there is a signal of the "T" nucleotide (red), which is high enough too. The second strongest signal is the thing we call _Alternative mutation_.

![An Alternative mutation example](/images/66814020/66814029.png "An Alternative mutation example")

It's very important to make _Alternative mutations_ clearly visible. To do this, you can use the function of the _Alternative mutation_. When the function is enabled and an _alternative mutation_ fits settings, the corresponding character will be replaced with the alternative one. The replacement causes the difference between the read and the reference character, which means, that the read character will be highlighted:

![A visible Alternative mutation](/images/66814020/66814043.png "A visible Alternative mutation")

_Alternative mutations_ settings are presented on the following picture:

![Settings of the function](/images/66814020/66814024.png "Settings of the function")_Show alternative mutations_ \- enable _Alternative mutations_ and show them if checked, disable and hide otherwise.

_Threshold_ - how high the second strongest signal (corresponding to the firsts strongest signal) should be to be visible. Look at the picture below. The height of the second signal is 75% of the height of the first signal. That means, that the _threshold_ value should be set to 75% (or below) to make this _alternative mutation_ visible.

![](/images/66814020/66814051.png)

_Update_ - click on this button to update the alignment corresponding to the set values.
