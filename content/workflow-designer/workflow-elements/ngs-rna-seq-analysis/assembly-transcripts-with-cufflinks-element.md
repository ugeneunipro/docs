---
title: "Assembly Transcripts with Cufflinks Element"
weight: 200
---


# Assembly Transcripts with Cufflinks Element

Cufflinks accept aligned RNA-Seq reads and assemble the alignments into a parsimonious set of transcripts. Cufflinks then estimate the relative abundances of these transcripts based on how many reads support each one, taking into account biases in library preparation protocols.

**Element type:** cufflinks

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Output directory**

Directory to save MACS output files.



**out-dir**

_string_

**Reference annotation**

Tells Cufflinks to use the supplied reference annotation to estimate isoform expression. Cufflinks will not assemble novel transcripts and the program will ignore alignments not structurally compatible with any reference transcript.



**ref-annotation**

_string_

**RABT annotation**

Tells Cufflinks to use the supplied reference annotation to guide Reference Annotation Based Transcript (RABT) assembly. Reference transcripts will be tiled with faux-reads to provide additional information in an assembly. The output will include all reference transcripts as well as any novel genes and isoforms that are assembled.



**rabt-annotation**

_string_

**Library type**

Specifies RNA-Seq protocol.

Standart Illumina

**library-type**

_numeric_

**Mask file**

Ignore all reads that could have come from transcripts in this file. It is recommended to include any annotated rRNA, mitochondrial transcripts other abundant transcripts you wish to ignore in your analysis in this file. Due to variable efficiency of mRNA enrichment methods and rRNA depletion kits, masking these transcripts often improves the overall robustness of transcript abundance estimates.



**mask-file**

_string_

**Multi-read correct**

Tells Cufflinks to do an initial estimation procedure to more accurately weight reads mapping to multiple locations in the genome.

False

**multi-read-correct**

_boolean_

**Min isoform fraction**

After calculating isoform abundance for a gene, Cufflinks filters out transcripts that it believes are very low abundance, because isoforms expressed at extremely low levels often cannot reliably be assembled, and may even be artifacts of incompletely spliced precursors of processed transcripts. This parameter is also used to filter out introns that have far fewer spliced alignments supporting them.

0.1

**min-isoform-fraction**

_numeric_

**Frag bias correct**

Providing Cufflinks with a multifasta file via this option instructs it to run the bias detection and correction algorithm which can significantly improve the accuracy of transcript abundance estimates.



**frag-bias-correct**

_string_

**Pre-mRNA fraction**

Some RNA-Seq protocols produce a significant amount of reads that originate from incompletely spliced transcripts, and these reads can confound the assembly of fully spliced mRNAs. Cufflinks use this parameter to filter out alignments that lie within the intronic intervals implied by the spliced alignments. The minimum depth of coverage in the intronic region covered by the alignment is divided by the number of spliced reads, and if the result is lower than this parameter value, the intronic alignments are ignored.

0.15

**pre-mrna-fraction**

_numeric_

**Cufflinks tool path**

The path to the Cufflinks external tool in UGENE.

default

**path**

_string_

**Temporary directory**

The directory for temporary files.

default

**tmp-dir**

_string_

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input reads

**Name in Workflow File:** in-assembly

**Slots:**

Slot In GUI

Slot in **Workflow** File

Type

**Assembly data**

assembly

_assembly_

**Source url**

url

_string_

And 1 _output port_:

**Name in GUI:** Output annotations

**Name in **Workflow** File:** out-annotations

**Slots:**

Slot In GUI

Slot in **Workflow** File

Type

**Isoform-level expression values**

isolevel.slot

_ann\_table_
