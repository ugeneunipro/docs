---
title: "Posterior Actions"
weight: 200
---

# Posterior Actions

This tab contains actions that could be processed for found primers.

![](/images/96665900/96665902.png)

Check Complementarity
---------------------

The "Check Complementarity" subprocess is responsible for filtering the result primers. If a primer pair has self-dimers or heterodimers with **dimer length**/**dimer GC-content** equal to or exceeding the set limits, this primer pair will be filtered out and will not be considered as a result of the Primer3 calculation.

If "Check Complementarity" is enabled, the result report will contain an additional table that shows filtered primers and explains why they have been filtered:

![](/images/96665900/96665905.png)

Primer pairs on **green** lines fit the set parameters and have not been filtered.

Primer pairs on **red** lines have problematic values, which are marked in bold — and that is why they have been excluded from the result. For example, the first pair has been filtered out because their heterodimer has a GC-content that is too high (75%).

The same report but in CSV format can be received by checking **Generate CSV report**.