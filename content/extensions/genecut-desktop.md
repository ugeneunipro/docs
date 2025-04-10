---
title: "GeneCut Desktop"
weight: 3600
---

# GeneCut Desktop

The GeneCut desktop tool for UGENE aims to display the results of [the GeneCut tool](http://genecut.unipro.ru/) appropriately.

First of all, you need to sign in using your login and password in GeneCut.

![](/images/88080434/88080445.png)

You will see the following page:
![](/images/88080434/88080446.png)

Now, there is the possibility to open the current sequence in GeneCut and continue working with the web service. To do this, click "Open this sequence in GeneCut."

However, the main feature is to view the results of all calculations you made in GeneCut. To display them, click "Fetch results." You can now see all calculations, their dates, and result statuses:
![](/images/88080434/88080453.png)

After clicking on the result, you will see the following options:

- Remove selected report - Remove the report and all data of the selected calculation.
- Get the input sequence - Download the sequence this calculation was started with.
- Open full report in GeneCut - Open the full report of the selected result in the browser.
- Get the result sequence - Download the result sequence (optimized, if some of the "Optimization" steps have been selected) with the long blocks/oligonucleotides marked as annotations (if some of the "Disassembly" steps have been selected). This step is available only if the calculation has been completed correctly.
- Compare input and result sequence - Open input and result sequences as alignment for you to see differences. This feature can be useful if some of the "Optimization" steps have been selected. This step is available only if the calculation has been completed correctly.