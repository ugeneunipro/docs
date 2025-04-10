---
title: "Functions Supported for Multiple Alignment Data"
weight: 100
---

# Functions Supported for Multiple Alignment Data

*   **createAlignment** (Sequence seq1, Sequence seq2, ...) — Returns the alignment created from the sequences.
*   **addToAlignment** (MAlignment aln, Sequence seq, int row = -1) — Adds the sequence to the specified row of the alignment. If the “row” parameter is not specified, the sequence is added to the end of the alignment.
*   **sequenceFromAlignment** (MAlignment aln, int row) — Returns the sequence from the specified row of the alignment.
*   **findInAlignment** (MAlignment aln, Sequence seq) — Searches the alignment for the specified sequence. Returns the number of the row if the sequence has been found or “-1” if it hasn’t been found.
*   **findInAlignment** (MAlignment aln, QString name) — Searches the alignment for a sequence with the specified name.
*   **removeFromAlignment** (MAlignment aln, int row) — Removes a sequence from the specified row of the alignment.
*   **rowNum** (MAlignment aln) — Returns the number of rows in the alignment.
*   **columnNum** (MAlignment aln) — Returns the length of the alignment.
*   **alignmentAlphabetType** (MAlignment aln) — Returns the alignment’s alphabet type.