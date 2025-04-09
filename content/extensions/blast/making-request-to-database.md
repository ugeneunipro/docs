---
title: "Making Request to Database"
weight: 200
---


# Making Request to Database

To make a request to a local BLAST database do the following:

*   Open _Tools ‣ BLAST ‣ BLAST search_.

If there is a sequence opened you can also initiate the request to a local BLAST database from the _Sequence View_:

*    Select the _Analyze ‣ Query with local BLAST_ item in the context menu or in the _Actions_ the main menu.

The _Request to local BLAST database_ dialog will appear:


![](/images/65930723/65930724.png)

The following general options are available:

_Select search -_ here you should select the tool you would like to use. If the query sequence is a nucleotide sequence then _blastn_, _blastx_ and _tblastx_ items are available. For a protein sequence, the items are _blastp_ and _tblastn_.

_Expectation value -_ this option specifies the statistical significance threshold for reporting matches against database sequences. Lower expect thresholds are more stringent, leading to fewer chance matches being reported.

_Culling limit -_ the maximum number of hits that will be shown (not equal to a number of annotations). The maximum available number is 5000.

_Search for short, nearly exact matches -_ automatically adjusts the word size and other parameters to improve results for short queries.

_Megablast -_ select this option to compare queries with closely related sequences. It works best if the target percent identity is 95% or more, but it is very fast.

_Database path -_ path to the database files.

_Base name for BLAST DB files -_ the base name for the BLAST database files.

You can see the description of the annotation saving parameters [_here_](https://ugene.unipro.ru/wiki/display/UUOUM16/Creating+Annotation).

The following advanced parameters are available:


![](/images/65930723/65930725.png)

_Word size -_ the size of the subsequence parameter for the initiated search.

_Gap costs -_ costs to create and extend a gap in an alignment. Increasing the Gap costs will result in alignments which decrease the number of Gaps introduced.

_Match scores -_ reward and penalty for matching and mismatching bases.

_Filters -_ filters for regions of low compositional complexity and repeat elements of the human’s genome.

_Masks for lookup table only_ — this option masks only for purposes of constructing the lookup table used by BLAST so that no hits are found based upon low-complexity sequence or repeats (if repeat filter is checked).

_Mask lower case letters_ — with this option selected you can cut and paste a FASTA sequence in upper case characters and denote areas you would like filtered with lower case.

The view of the _Advanced options_ tab depends on the selected search. For the _blastn_ search, it looks like in the picture above. When the _blastx_ search is selected in the general options, the view of the _Advanced options_ tab is the following:


![](/images/65930723/65930726.png)

As you can see there is no _Match scores_ option, but there are _Threshold_, _Matrix, Composition-based statistics_ and _Service_ options.

_Threshold -_ threshold for extending hits.

_Matrix_ — key element in evaluating the quality of pair-wise sequence alignment is the “substitution matrix”, which assigns a score for aligning any possible pair of residues.

_Service_ — blastp service which needs to be performed: plain, psi or phi.

_Composition-based statistics_ - composition-based statistics.

When the _tblastx_ search is selected in the general options, the view of the _Advanced options_ tab is the following:


![](/images/65930723/65930727.png)

The following extension options are available:


![](/images/65930723/65930728.png)

_For gapped alignment -_ X dropoff value (in bits) for gapped alignment.

_For ungapped alignment -_ X dropoff value (in bits) for ungapped alignment.

_For final gapped alignment -_ X dropoff value (in bits) for final gapped alignment.

_Multiple hits window size -_ multiple hits window size.

_Perform gapped alignment -_ performs gapped alignment.
