---
title: "Functions Supported for Multiple Alignment Data"
weight: 1
---


# Functions Supported for Multiple Alignment Data

*   **createAlignment** (Sequence seq1, Sequence seq2, ...) — returns the alignment created from the sequences.
*   **addToAlignment** (MAlignment aln, Sequence seq, int row = -1) — adds the sequence to the specified row of the alignment. If the “row” parameter is not specified the sequence is added to the end of the alignment.
*   **sequenceFromAlignment** (MAlignment aln, int row) — returns the sequence from the specified row of the alignment.
*   **findInAlignment** (MAlignment aln, Sequence seq) — searches the alignment for the specified string. Return the number of the row if the sequence has been found or “-1” if it hasn’t been found.
*   **findInAlignment** (MAlignment aln, QString name) — searches the alignment for a sequence with the specified name.
*   **removeFromAlignment** (MAlignment aln, int row) — removes a sequence from the specified row of the alignment.
*   **rowNum** (MAlignment aln) — returns the number of rows in the alignment.
*   **columnNum** (MAlignment aln) — returns the length of the alignment.
*   **alignmentAlphabetType** (MAlignment aln) — returns the alignment’s alphabet.
