---
title: "Primer3 (no target sequence)"
weight: 1
---


# Primer3 (no target sequence)

It is also possible to run Primer3 without target sequence. To do so, click Tools → Primer → Primer3 (no target sequences):![](/images/96666247/96666250.png)

The same dialog as for a usual Primer3 calculation will be opened:

![](/images/96666247/96666251.png)

The main diference is that you cannot choose task - only **check\_primers** is avaliable (which is obvious, because you need to provide at least some primers to have a result). [RTPCR Primer Design](rtpcr-primer-design.md) and [Posterior Actions](posterior-actions.md) tabs are also disabled, as far as their executions expect target sequences. After performing the calculation, you will get the result sequence with your input primers:

![](/images/96666247/96666257.png)

Result primers have the same qualifiesr as in a [regular Primer3 calculation](https://doc.ugene.net/wiki/pages/viewpage.action?pageId=65930919#Primer3-p3quals).
