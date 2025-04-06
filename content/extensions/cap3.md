---
title: "CAP3"
weight: 1
---


# CAP3

[CAP3 (CONTIG ASSEMBLY PROGRAM Version 3)](http://genome.cshlp.org/content/9/9/868.full) is a sequence assembly program for small-scale assembly with or without quality values. Click [this link](http://seq.cs.iastate.edu/) to open _CAP3_ homepage. _CAP3_ is embedded as an [_external tool_](external-tools-plugin.md) into UGENE.

Open _Tools ‣ Sanger data analysis_ submenu of the main menu.


![](/images/23331222/24117249.jpg)

Select the _Reads de novo assembly (with CAP3)_ item to use the _CAP3_.

The _Contig Assembly With CAP3_ dialog appears.


![](/images/4227725/4457139.png)

You can add or remove input files using _Add_ and _Remove_ buttons. To remove all files click the _Remove all_ button. _Input files_ are files with a long DNA reads in FASTA, FASTQ, SCF or ABI formats. At least one input file should be added. Input a _Result contig_ name and press the _Run_ button. _CAP3_ produces assembly results in the ACE file format (”.ace”). The file contains one or several contigs assembled from the input reads.

The quality scores for FASTA sequences can be provided in an additional file. The file must be located in the same folder as the original sequences and have the same name as FASTA file, but another extension: **_.qual_**.

Also you can change the following advanced parameters:


![](/images/4227725/4457140.png)

_Clipping for poor regions_ parameters:

Clipping of a poor end region of a read is controlled by parameters _Base quality cutoff for clipping (-c)_ (the specified value should be more than 5), and _Clipping range (-y)_ (the specified value should be more than 5).

_Quality difference score of an overlap_ parameters:

_Base quality cutoff for differences (-b)_ — if an overlap contains a difference at bases of quality values q1 and q2, then the score at the difference is max(0, min(q1, q2) - b), where b is the specified value. The specified value should be more than 15. The difference score of an overlap is the sum of scores at each difference.

_Max qscore sum at differences (-d)_ — remove an overlap if its difference score is greater than the specified value. The specified value should be more than 20.

_Similarity score of an overlap_ parameters:

The following parameters are used to calculate the similarity score of an overlapping alignment:

_Match score factor (-m)_ — a match at bases of quality values q1 and q2 is given a score of m \* min(q1, q2), where m is the specified value. The specified value should be more than 0.

_Mismatch score factor (-n)_ — a mismatch at bases of quality values q1 and q2 is given a score of n \* min(q1, q2), where n is the specified value. The specified value should be less than 0.

_Gap penalty factor (-g)_ — a base of quality value q1 in a gap is given a score -g \* min(q1, q2), where g is the specified value; q2 is the quality value of the base in the other sequence right before the gap. The specified value should be more than 0.

The similarity score is caclulated as the sum of scores of each match, each mismatch and each gap. Based on this value and the following value some overlaps are removed:

_Overlap similarity score cutoff (-s)_ — remove overlaps with similarity scores less than the specified value. The specified value should be more than 250.

_Length and percent identity of an overlap_ parameters:

_Overlap length cutoff (-o)_ — minimum length of an overlap (in base pairs). The specified value should be more than 15 base pairs.

_Overlap percent identity cutoff (-p)_ — minimum percent identity of an overlap. The specified value should be more than 65%.

_Other parameters_:

_Maximum number of word matches (-t)_ — an upper limit of word matches between a read and other reads. Increasing the value would result in more accuracy, however this could slow down the program. The specified value should be more than 0.

_Band expansion size (-a)_ — a number of bases to expand a band of diagonals for an overlapping alignment between two sequence reads. The specified value should be more than 10.

_Max gap length in any overlap (-f)_ — reject overlaps with a gap longer than the specified value. A small value may cause the program to remove true overlaps and to produce incorrect results. This option may be used by the user to split reads from alternative splicing forms into separate contigs. The specified value should be more than 1.

_Assembly reverse reads (-r)_ — consider reads in reverse orientation for assembly. The default value is “checked”.
