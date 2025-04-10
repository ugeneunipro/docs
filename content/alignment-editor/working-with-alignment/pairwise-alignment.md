---
title: "Pairwise Alignment"
weight: 1000
---

# Pairwise Alignment

To align two sequences, navigate to the _Pairwise Alignment_ tab in the _Options Panel_:

![](/images/65929675/96666065.png)

Select two sequences from the original alignment, adjust the parameters, and click on the _Align_ button. The following parameters are available:

### Sequences

The first and second sequences for the _Pairwise Alignment_.

### Algorithm

The algorithm for the _Pairwise Alignment_. There are two algorithms:

1.  **KAlign** - provided by the Kalign tool (integrated as an External Tool, check the [Data Analysis Tools page](https://doc.ugene.net/wiki/display/UM/Data+Analysis+Tools) for details). This tool uses the **Wu-Manber** string-matching algorithm. The algorithm details are described in the corresponding publication \[Lassmann T, Sonnhammer EL. Kalign—an accurate and fast multiple sequence alignment algorithm. BMC Bioinformatics. 2005 Dec 12;6:298. doi: 10.1186/1471-2105-6-298. PMID: 16343337; PMCID: PMC1325270 [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1325270/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1325270/)\]. The algorithm has the following parameters:
    *   _Gap open penalty_ - indicates the penalty applied for opening a gap. The penalty must be negative.
    *   _Gap extension penalty_ - indicates the penalty applied for extending a gap.
    *   _Terminal gap penalty_ - the penalty for extending gaps from the N/C terminal of protein or 5'/3' terminal of nucleotide sequences.
2.  **Smith-Waterman** - the same algorithm used for the [Smith-Waterman Search](https://doc.ugene.net/wiki/display/UM/Smith-Waterman+Search) (check the page for algorithm details - the alignment process works the same way as the searching process). The following parameters are available:
    *   _Algorithm version_ - version of the algorithm implementation. Non-classic versions produce the same results as classic but much faster. To use these optimizations, your system must support [SSE2](https://en.wikipedia.org/wiki/SSE2).
    *   _Scoring matrix_ - the scoring matrix.
    *   _Gap open penalty_ - the penalty for opening a gap.
    *   _Gap extension penalty_ - the penalty for extending a gap.

### Output settings

Settings for the output file:

*   _In the new window_ - create a new alignment and open it if checked, or just align two sequences of the current alignment if it is not.
*   _Output file_ - the path to the result file.