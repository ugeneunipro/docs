---
title: "DNA Statistics"
weight: 300
---

# DNA Statistics

The _DNA Statistics_ plugin provides exportable statistical reports.

In the current UGENE version, the _DNA Statistics_ plugin only provides an _Alignment Grid Profile_ report. The _Alignment Grid Profile_ displays positional amino acid or nucleotide counts, highlighted according to the frequency of symbols in a row.

The original idea of the MSA Grid Profile is described in the following paper:

“Alberto Roca, Albert Almada and Aaron C Abajian: ProfileGrids as a new visual representation of large multiple sequence alignments: a case study of the RecA protein family, BMC Bioinformatics 2008, 9:554”

**Usage example:**

Open a sequence alignment in the _Alignment Editor_ and use the _Statistics ‣ Generate grid profile_ context menu item.

![](/images/65930700/65930701.png)

The dialog will appear:

![](/images/65930700/65930702.png)

Here is a brief description of the options that can be set in the dialog:

- _Profile mode: Counts/Percents_ — select _Percents_ to have scores shown as percentages in the report.

- _Show scores for gaps_ — check this item if you want gap character (‘—’) statistics to be displayed in the report.

- _Show scores for symbols not used in alignment_ — if a symbol is not used in the alignment at all, it won’t be displayed in the report. Check this item to report all symbols of the alignment alphabet.

- _Skip gaps in consensus position increments_ — consensus ruler configuration. If checked, the gaps in the consensus will not lead to ruler increments.

- _Save profile to file_ — allows saving the profile to a file in HTML or CSV format. The CSV format is convenient for further processing in spreadsheet editors like Excel.

The resulting profile in HTML mode:

![](/images/65930700/65930703.png)