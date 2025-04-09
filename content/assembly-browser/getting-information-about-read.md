---
title: "Getting Information About Read"
weight: 300
---


# Getting Information About Read

A read displayed in the _Reads Area_ consists of the bases (A, C, G, T). It may also contain the N character that stays for an ambigous base. Depending on the value of the _Cigar_ parameter, the read can be shown partially or gaps can be inserted inside the read (see below).

By default when a read is hovered over in the _Reads Area_ a hint appears:


![](/images/65929817/65929818.png)

To disable this behaviour click the following button on the toolbar:


![](/images/65929817/65929819.png)

Or uncheck the _Show pop-up hint_ check box on the _Assembly Browser Settings_ tab of the _Options Panel_.

The hint shows the following information about the read:

*   Read name
*   Location
*   Length
*   Cigar
*   Strand
*   Read sequence

The operations in the _Cigar_ parameter are described as follows:

*   **M** — Alignment match (can be a sequence match or mismatch).

*   **I** — Insertion to the reference. Skipped when the read is aligned to the reference, i.e. it is not shown in the Reads Area, but is present in the read sequence.

*   **D** — Deletion from the reference. Gaps are inserted to the read when the read is aligned to the reference. For example:



![](/images/65929817/65929820.png)

*   **N** — Skipped region from the reference. Behaves as **D**, but has a different biological meaning: for mRNA-to-genome alignment it represents an intron.

*   **S** — Soft clipping (clipped sequences are present in the read sequence, i.e. behaves as **I**).

*   **H** — Hard clipping (clipped sequences are not present in the read sequence).

*   **P** — Padding (silent deletion from padded reference).

*   **\=** — Exact match to the reference.

*   **x** — Reference sequence mismatch.


To copy the information about the read to the clipboard, select the _Copy read information to clipboard_ item in the Reads Area context menu. Now you can paste it in any text editor.

To copy the current position of the read select the _Copy current position to clipboard_ item in the _Reads Area_ context menu.
