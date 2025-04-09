---
title: "Posterior Actions"
weight: 200
---


# Posterior Actions

This tab contains actions, which could be processed for found primers.

![](/images/96665900/96665902.png)

Check complementary
-------------------

The "Check complementary" subprocess is responsible for result primers filtering. If primer pair has selfdimers or heterodimer with **dimer length**/**dimer GC-content** more or equal, than was set, this primer will be filtered and won't be considered as a result of Primer3 calculation.

If "Check complementary" has been checked, the result report will contain the additional table, which shows filtered primers and why have they been filtered:

![](/images/96665900/96665905.png)

Primer pairs on **green** lines are fit to the set parameters and have not been filtered.

Primer pairs on **red** lines have some problem values, which are marked in bold - and that is why they have been excluded from the result. For example, the first pair has been filtered, because their heterodimer has too hight GC-content (75%).

The same report but in CSV format you can recieve by checking **Generate CSV report**.
