---
title: "RTPCR Primer Design"
weight: 300
---

# RTPCR Primer Design

This feature allows users to search for primer pairs that span introns on the genomic sequence or exon junctions on the mRNA sequence.

Note that RT-PCR design is only available for mRNA/cDNA sequences with annotated exons. There are several ways to obtain the cDNA for a corresponding DNA sequence.

* From NCBI or ENSEMBL databases.  
  For example, one can download the **_TMPRSS2 transcript variant 1_** from NCBI Genbank using identifier [NM\_001135099.1](http://www.ncbi.nlm.nih.gov/nuccore/NM_001135099.1).
  This can also be done from UGENE using the option [Access remote database](../../basic-functions/fetching-data-from-remote-database) or [Search NCBI Genbank](../../basic-functions/searching-ncbi-genbank).

* Align the genomic and cDNA sequences using a [spliced aligner](../spliced-alignment-mrna-and-cdna).
  For this option, one must have both genomic and cDNA sequences.
  In UGENE, the spliced alignment can be performed using the [Spidey tool](../spliced-alignment-mrna-and-cdna).
  To run the alignment, open the genomic sequence and select the action _Align_ ‣ _Align to mRNA sequence_.
  The generated exon annotations can then be exported using the action _Export_ ‣ _Export sequence of selected annotations_.

To design primers for your mRNA sequence, go to the RT-PCR tab of the _Primer Designer_ dialog:

![](/images/65930921/65930922.png)

The following parameters are available:

_Exon annotation name_

To detect exon boundaries, UGENE searches for exonic annotations. This option allows setting a custom name for annotations denoting exons. The default value is "exon."

_Minimum exon junction overlap size_

If checked, then only the pairs with at least one of the primers overlapping the exon junction in the mRNA sequence will be selected.

At 5' side (bp)

Minimum overlap size on the 5' side of the exon junction. The default is 5 bp.

At 3' side (bp)

Minimum overlap size on the 3' side of the exon junction. The default is 5 bp.

_Exon range_

This option allows limiting the sequence region where the primers are searched for. For example, setting the value "3-5" will limit the search to a sequence region consisting of exons 3, 4, and 5 of the transcript, as defined by the order in the sequence. The default value is an empty string, which means that there are no limitations.

_Span at least one intron_

This option ensures that the primer product spans an intron on the genomic sequence, i.e., the forward and reverse primers must be located in different exons. The option is enabled by default.

_Max number of pairs to query_

The algorithm applied in RT-PCR primer design first searches for all available primers in a given sequence. Then it filters the detected pairs to make sure that they satisfy the selected configuration. This option allows setting the maximum number of pairs for the initial search query. A larger number will result in increased sensitivity but also in a longer running time. The default value is 1000.

**Important**: Using the **RT-PCR** primer design tab will reset the values set in the _Excluded regions_ and _Targets_ of the **Main** configuration tab. Additionally, if the _Exon range_ option is set, the defined sequence region will be ignored.