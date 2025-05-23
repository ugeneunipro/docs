---
title: "Exporting Coverage"
weight: 300
---

# Exporting Coverage

To export the coverage of the assembly, select the _Export coverage_ item in the _Consensus Area_ context menu.

The _Export Coverage_ dialog appears:

![](/images/65929844/65929845.png)

The following parameters are available:

*   _Export to_ - select the result file path,
*   _Format_ - assembly coverage can be saved in three different formats:
    *   Bedgraph - the coverage is shown by columns. If several columns in a row have the same occurrence, they will be combined into one column.
    *   Histogram - shows coverage by frequency of occurrence. That is, a row is deciphered as a column number **N** with coverage **X** occurring in an assembly of length **L**, and the total occurrence rate is **Z**:
        ![](/images/65929844/96666051.png)
    *   Per base - similar to BaseGraph, but without columns merging.
        *   Export coverage value - add coverage for each base (how many reads are in the column).
        *   Export bases quantity - add the amount of A, C, G, and T.
*   _Threshold_ - consider the column only if it has more reads than set by this parameter.
*   _Compress the file_ - archive as **.gz**.