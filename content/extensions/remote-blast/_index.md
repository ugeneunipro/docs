---
title: "Remote BLAST"
weight: 600
---


# Remote BLAST

The _Remote BLAST_ plugin provides a capability to annotate sequences with information stored in the [NCBI BLAST](http://blast.ncbi.nlm.nih.gov/Blast.cgi) remote database.

To perform a remote database search open a _Sequence View_, select a sequence region to analyze and click the _Analyze ‣ Query NCBI BLAST database_ context menu item. If a region is not selected the whole sequence will be analyzed.


![](/images/65930710/65930711.png)

The following dialog will appear where you can choose the search options:


![](/images/65930710/65930712.png)

General options are:

_Select the search type_ — in the remote databases the _blastn_ search is used for nucleotide sequences, _blastp_ and _cdd_ searches are used for amino sequences.

UGENE also provides a way to use _blastp_ and _cdd_ searches for nucleotide sequences. This is achieved by translating the nucleotide sequence into the amino sequences.

When a sequence is translated the translation table from the active _Sequence View_ is used. Finally, all 6 translations are used to query the remote database with the selected _blastp_ or _cdd_ search.

_Expectation value_ — this option specifies the statistical significance threshold for reporting matches against database sequences. Lower expect thresholds are more stringent, leading to fewer chance matches being reported.

_Max hits_ — the maximum number of hits that will be shown (not equal to number of annotations). The maximum availablle number is 5000.

_Database_ — the target database.

_Search for short, nearly exact matches_ — automatically adjusts the word size and other parameters to improve results for short queries.

_Megablast_ — select this option to compare query with closely related sequences. It works best if the target percent identity is 95% or more, but it is very fast.

You can see the description of the annotation saving parameters [_here_](../../sequence-view/manipulating-annotations/creating-annotation).

_Search timeout_ — the remote task terminated if the timeout is reached.

There is a little difference in default values of parameters between [NCBI Nucleotide BLAST](http://blast.ncbi.nlm.nih.gov/Blast.cgi?PROGRAM=blastn&PAGE_TYPE=BlastSearch&LINK_LOC=blasthome) web interface and UGENE:

*   The web interface uses the _megablast_ option by default: the search is fast, but only highly similar sequences are found.
*   UGENE ignores the option by default: the search may take more time, but all somewhat similar sequences are found.

Check the _Megablast_ option, if you want exactly the same results to be found in UGENE as you had in the NCBI web interface.

Also there is _Advanced options_ tab:


![](/images/65930710/65930713.png)

The view of the _Advanced options_ tab depends on the selected search. For the _blastn_ search it looks like on the picture above.

_Word size_ — the size of the subsequence parameter for the initiated search.

_Gap costs_ — costs to create and extend a gap in an alignment. Increasing the Gap costs will result in alignments which decrease the number of Gaps introduced.

_Match scores_ — reward and penalty for matching and mismatching bases.

_Entrez query_ — a BLAST search can be limited to the result of an _Entrez query_ against the database chosen. This restricts the search to a subset of entries from that database fitting the requirement of the _Entrez query_. Examples are given below:

_protease NOT hiv1\[organism\]_ — this will limit a BLAST search to all proteases, except those in HIV 1.

_1000:2000\[slen\]_ — this limits the search to entries with lengths between 1000 to 2000 bases for nucleotide entries, or 1000 to 2000 residues for protein entries.

_Mus musculus\[organism\] AND biomol\_mrna\[properties\]_ — this limits the search to mouse mRNA entries in the database. For common organisms, one can also select from the pulldown menu.

_10000:100000\[mlwt\]_ — this is yet another example usage, which limits the search to protein sequences with calculated molecular weight between 10 kD to 100 kD.

_src specimen voucher\[properties\]_ — this limits the search to entries that are annotated with a /specimen\_voucher qualifier on the source feature.

_all\[filter\] NOT enviromnental sample\[filter\] NOT metagenomes\[orgn\]_ — this excludes sequences from metagenome studies and uncultured sequences from anonymous environmental sample studies.

For help in constructing _Entrez queries_ see the [Entrez Help document](http://www.ncbi.nlm.nih.gov/books/NBK3837/).

_Filters_ — filters for regions of low compositional complexity and repeat elements of the human’s genome.

_Masks for lookup table only_ — this option masks only for purposes of constructing the lookup table used by BLAST so that no hits are found based upon low-complexity sequence or repeats (if repeat filter is checked).

_Mask lower case letters_ — with this option selected you can cut and paste a FASTA sequence in upper case characters and denote areas you would like filtered with lower case.

_Filter by_ — filters results by accession, by definition of annotations or by id.

_Select result by_ — selects results by EValue or by score.

When the _blastp_ search is selected in the general options, the view of the _Advanced options_ tab is the following:


![](/images/65930710/65930714.png)

As you can see there is no _Match scores_ option, but there are _Matrix_ and _Service_ options.

_Matrix_ — key element in evaluating the quality of a pair-wise sequence alignment is the “substitution matrix”, which assigns a score for aligning any possible pair of residues.

_Service_ — blastp service which needs to be performed: plain, psi or phi.

The _Advanced options_ tab is not available when the _cdd_ search is selected.
