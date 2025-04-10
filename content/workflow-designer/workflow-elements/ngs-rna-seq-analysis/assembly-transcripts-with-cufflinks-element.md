---
title: "Assembly Transcripts with Cufflinks Element"
weight: 200
---

# Assembly Transcripts with Cufflinks Element

Cufflinks accepts aligned RNA-Seq reads and assembles these alignments into a parsimonious set of transcripts. Cufflinks then estimates the relative abundances of these transcripts based on the number of reads supporting each one, taking into account biases in library preparation protocols.

**Element type:** cufflinks

## Parameters

| Parameter                | Description                                                                                                                                                                             | Default value     | Parameter in Workflow File | Type      |
|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|----------------------------|-----------|
| **Output directory**     | Directory to save MACS output files.                                                                                                                                                    |                   | **out-dir**                | _string_  |
| **Reference annotation** | Use the supplied reference annotation to estimate isoform expression. Novel transcripts will not be assembled. Alignments not compatible with any reference transcript are ignored.     |                   | **ref-annotation**         | _string_  |
| **RABT annotation**      | Use the supplied reference annotation to guide Reference Annotation Based Transcript (RABT) assembly. Adds faux reads. Output includes reference transcripts and any novel transcripts. |                   | **rabt-annotation**        | _string_  |
| **Library type**         | Specifies RNA-Seq protocol.                                                                                                                                                             | Standard Illumina | **library-type**           | _numeric_ |
| **Mask file**            | Reads from transcripts in this file are ignored (e.g., rRNA, mitochondrial). Masking improves the robustness of abundance estimates.                                                    |                   | **mask-file**              | _string_  |
| **Multi-read correct**   | Enable procedure to better weight reads mapping to multiple genome locations.                                                                                                           | False             | **multi-read-correct**     | _boolean_ |
| **Min isoform fraction** | Filters out very low abundance transcripts that may be unreliable or artifacts. Also filters introns with few supporting alignments.                                                    | 0.1               | **min-isoform-fraction**   | _numeric_ |
| **Frag bias correct**    | Run bias correction algorithm using the provided multi-FASTA file of the genome. Improves abundance estimates.                                                                           |                   | **frag-bias-correct**      | _string_  |
| **Pre-mRNA fraction**    | Filters intronic alignments if they are likely pre-mRNA. The value defines the threshold for intron depth vs. splice reads.                                                             | 0.15              | **pre-mrna-fraction**      | _numeric_ |
| **Cufflinks tool path**  | Path to the Cufflinks external tool in UGENE.                                                                                                                                           | default           | **path**                   | _string_  |
| **Temporary directory**  | Directory for temporary files.                                                                                                                                                          | default           | **tmp-dir**                | _string_  |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Input reads  
**Name in Workflow File:** in-assembly  
**Slots:**

| Slot In GUI       | Slot in Workflow File | Type       |
|-------------------|-----------------------|------------|
| **Assembly data** | assembly              | _assembly_ |
| **Source url**    | url                   | _string_   |

And 1 _output port_:

**Name in GUI:** Output annotations  
**Name in Workflow File:** out-annotations  
**Slots:**

| Slot In GUI                         | Slot in Workflow File | Type        |
|-------------------------------------|-----------------------|-------------|
| **Isoform-level expression values** | isolevel.slot         | _ann_table_ |