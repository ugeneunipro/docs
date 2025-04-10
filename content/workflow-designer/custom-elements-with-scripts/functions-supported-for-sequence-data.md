---
title: "Functions Supported for Sequence Data"
weight: 200
---

# Functions Supported for Sequence Data

* **subsequence** (Sequence seq, int beg, int end) - returns the subsequence between the "beg" and "end" parameters.
* **complement** (Sequence seq) - returns the complement of the sequence.
* **translate** (Sequence seq, int offset = 0) - returns one of the three sequence translations. The "offset" parameter determines which one is returned.
* **size** (Sequence seq) - returns the length of the sequence.
* **getName** (Sequence seq) - returns the name of the sequence.
* **alphabetType** (Sequence seq) - returns the alphabet of the sequence.
* **charAt** (Sequence seq, int ind) - returns the symbol located at the "ind" position of the sequence.
* **hasQuality** (Sequence seq) - determines whether the sequence has the "Quality" parameter.
* **getMinimumQuality** (Sequence seq) - returns the minimum value of the "Quality".
* **isAmino** (Sequence seq) - returns true if it is an amino acid sequence.
* **concatSequence** (Sequence1 seq1, Sequence2 seq2,...) - returns one sequence consisting of all input sequences.
* **sequenceFromText** (QString " ") - returns the sequence consisting of the input text.