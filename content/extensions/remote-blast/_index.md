---
title: "Remote BLAST"
weight: 600
---

# Remote BLAST

The _Remote BLAST_ plugin provides the capability to annotate sequences with information stored in the [NCBI BLAST](http://blast.ncbi.nlm.nih.gov/Blast.cgi) remote database.

To perform a remote database search, open a _Sequence View_, select a sequence region to analyze, and click the _Analyze ‣ Query NCBI BLAST database_ context menu item. If a region is not selected, the whole sequence will be analyzed.

![](/images/65930710/65930711.png)

The following dialog will appear where you can choose the search options:

![](/images/65930710/65930712.png)

General options are:

- _Select the search type_ — In the remote databases, the _blastn_ search is used for nucleotide sequences, while _blastp_ and _cdd_ searches are used for amino acid sequences.

UGENE also provides a way to use _blastp_ and _cdd_ searches for nucleotide sequences. This is achieved by translating the nucleotide sequence into amino acid sequences.

When a sequence is translated, the translation table from the active _Sequence View_ is used. Finally, all six translations are used to query the remote database with the selected _blastp_ or _cdd_ search.

- _Expectation value_ — This option specifies the statistical significance threshold for reporting matches against database sequences. Lower expect thresholds are more stringent, leading to fewer chance matches being reported.

- _Max hits_ — The maximum number of hits that will be shown (not equal to the number of annotations). The maximum available number is 5000.

- _Database_ — The target database.

- _Search for short, nearly exact matches_ — Automatically adjusts the word size and other parameters to improve results for short queries.

- _Megablast_ — Select this option to compare the query with closely related sequences. It works best if the target percent identity is 95% or more, but it is very fast.

You can see the description of the annotation saving parameters [_here_](../../sequence-view/manipulating-annotations/creating-annotation).

- _Search timeout_ — The remote task is terminated if the timeout is reached.

There is a slight difference in default values of parameters between the [NCBI Nucleotide BLAST](http://blast.ncbi.nlm.nih.gov/Blast.cgi?PROGRAM=blastn&PAGE_TYPE=BlastSearch&LINK_LOC=blasthome) web interface and UGENE:

- The web interface uses the _megablast_ option by default: the search is fast but only finds highly similar sequences.
- UGENE ignores the option by default: the search may take more time, but it finds all somewhat similar sequences.

Check the _Megablast_ option if you want exactly the same results to be found in UGENE as you had in the NCBI web interface.

There is also an _Advanced options_ tab:

![](/images/65930710/65930713.png)

The view of the _Advanced options_ tab depends on the selected search. For the _blastn_ search, it looks like the picture above.

- _Word size_ — The size of the subsequence parameter for the initiated search.

- _Gap costs_ — Costs to create and extend a gap in an alignment. Increasing the gap costs will result in alignments that decrease the number of gaps introduced.

- _Match scores_ — Reward and penalty for matching and mismatching bases.

- _Entrez query_ — A BLAST search can be limited to the result of an _Entrez query_ against the chosen database. This restricts the search to a subset of entries from that database fitting the requirement of the _Entrez query_. Examples are given below:

  - _protease NOT hiv1\[organism\]_ — This will limit a BLAST search to all proteases, except those in HIV 1.
  - _1000:2000\[slen\]_ — This limits the search to entries with lengths between 1000 to 2000 bases for nucleotide entries or 1000 to 2000 residues for protein entries.
  - _Mus musculus\[organism\] AND biomol\_mrna\[properties\]_ — This limits the search to mouse mRNA entries in the database. For common organisms, one can also select from the pulldown menu.
  - _10000:100000\[mlwt\]_ — This is yet another example usage, which limits the search to protein sequences with calculated molecular weights between 10 kD to 100 kD.
  - _src specimen voucher\[properties\]_ — This limits the search to entries that are annotated with a /specimen\_voucher qualifier on the source feature.
  - _all\[filter\] NOT environmental sample\[filter\] NOT metagenomes\[orgn\]_ — This excludes sequences from metagenome studies and uncultured sequences from anonymous environmental sample studies.

For help in constructing _Entrez queries_, see the [Entrez Help document](http://www.ncbi.nlm.nih.gov/books/NBK3837/).

- _Filters_ — Filters for regions of low compositional complexity and repeat elements of the human genome.

- _Masks for lookup table only_ — This option masks only for purposes of constructing the lookup table used by BLAST so that no hits are found based upon low-complexity sequences or repeats (if repeat filter is checked).

- _Mask lower case letters_ — With this option selected, you can cut and paste a FASTA sequence in uppercase characters and denote areas you would like filtered with lowercase.

- _Filter by_ — Filters results by accession, by definition of annotations, or by id.

- _Select result by_ — Selects results by EValue or by score.

When the _blastp_ search is selected in the general options, the view of the _Advanced options_ tab is as follows:

![](/images/65930710/65930714.png)

As you can see, there is no _Match scores_ option, but there are _Matrix_ and _Service_ options.

- _Matrix_ — A key element in evaluating the quality of a pair-wise sequence alignment is the “substitution matrix”, which assigns a score for aligning any possible pair of residues.

- _Service_ — The blastp service which needs to be performed: plain, psi, or phi.

The _Advanced options_ tab is not available when the _cdd_ search is selected.