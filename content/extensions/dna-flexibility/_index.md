---
title: "DNA Flexibility"
weight: 200
---

# DNA Flexibility

To search for regions of high DNA helix flexibility in a DNA sequence:

1. Open the sequence in the _Sequence View_.
2. Right-click and select _Analyze → Find high DNA flexibility regions_.

> 🧬 **Note:** Only the **standard DNA alphabet** is supported: `A`, `C`, `G`, `T`, and `N`.

---

## Settings Dialog

The following dialog appears:

![](/images/65930694/65930695.png)

---

## Method

The analysis uses a **sliding window** approach. For each window:

- If **2 or more consecutive windows** have average flexibility **above the threshold**, the region is **annotated**.
- The **average flexibility** for a window is calculated as:

Average = (Sum of dinucleotide flexibility angles in the window) / (window size - 1)

## Flexibility Angles Table

| **Dinucleotide** | **Angle** | **Dinucleotide** | **Angle** |
|------------------|-----------|------------------|-----------|
| AA               | 7.6       | CA               | 14.6      |
| AC               | 10.9      | CC               | 7.2       |
| AG               | 8.8       | CG               | 11.1      |
| AT               | 12.5      | CT               | 8.8       |
| GA               | 8.2       | TA               | 25.0      |
| GC               | 8.9       | TC               | 8.2       |
| GG               | 7.2       | TG               | 14.6      |
| GT               | 10.9      | TT               | 7.6       |

---

## Handling Unknown Bases (N)

If the sequence contains ambiguous base `N`, the following minimum angle values are used:

- **CN, NC, GN, NG, NN** → _7.2_
- **AN, NA, TN, NT** → _7.6_
