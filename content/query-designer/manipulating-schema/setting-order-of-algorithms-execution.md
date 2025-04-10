---
title: "Setting Order of Algorithms Execution"
weight: 500
---

# Setting Order of Algorithms Execution

By default, the algorithms are executed in the same order as the corresponding _algorithm elements_ have been added to the _schema_:

1. The element with order 1 is executed.
2. The element with order 2 is executed. It uses the results obtained from step 1.
3. And so on.

Since each subsequent algorithm element uses the results obtained from the previous element, setting the order can affect efficiency. For example, the fewer results obtained in the first step, the faster the second algorithm is executed.

To change the order, use the _Set order_ submenu or _Up_ / _Down_ items in an _algorithm element_ context menu.

![](/images/65930644/65930645.png)