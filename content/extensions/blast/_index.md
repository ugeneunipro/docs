---
title: "BLAST"
weight: 700
---

# BLAST

The Basic Local Alignment Search Tool ([BLAST](http://blast.ncbi.nlm.nih.gov/)) finds regions of local similarity between sequences.

The program compares nucleotide or protein sequences to sequence databases and calculates the statistical significance of matches. BLAST can be used to infer functional and evolutionary relationships between sequences, as well as to help identify members of gene families.

From UGENE, you can use the following tools from the old BLAST package:

* **blastcmd** — The BlastDBCmd fetches protein or nucleotide sequences from a BLAST database based on a query.
* **makeblastdb** — Formats protein or nucleotide source databases before these databases can be searched by other BLAST tools.
* **blastn** — Searches a nucleotide database using a nucleotide query.
* **blastp** — Searches a protein database using a protein query.
* **blastx** — Searches a protein database using a translated nucleotide query.
* **tblastn** — Compares a protein query against a translated nucleotide database (all six reading frames).
* **tblastx** — Translates the query nucleotide sequence in all six possible frames and compares it against the six-frame translations of a nucleotide sequence database.
* **rpsblast** — RPS Blast: Reversed Position Specific Blast RPS-BLAST (Reverse PSI-BLAST) searches a query sequence against a database of profiles.

BLAST home page: [http://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastHome](http://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastHome)

To make _BLAST_ tools available from UGENE:

1. Install the required version of _BLAST_ on your system.
2. Set the paths to the executables you are going to use in the [_External tools_](external-tools-plugin.md) tab of the UGENE [_Application Settings_](ugene-application-settings.md) dialog.

After you’ve completed this configuration, you can access the tools from the _Tools ‣ BLAST_ submenu of the main menu.