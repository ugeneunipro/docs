---
title: "Workflow Elements"
weight: 1
---


# Workflow Elements

This section contains detailed description of all workflow elements presented in the Workflow Designer.

For each element you can find:

*   Description of the parameters used in the GUI
*   Corresponding parameters names used in a workflow file
*   Information about input and output ports

The type of a parameter can be one of the following:

**string**

A string.

**numeric**

A number.

**boolean**

A boolean data type. Available values are: true / false, 0 / 1 and yes / no.

A port’s slot type can be one of the following:

**sequence**

Biological sequence

**msa**

Multiple sequence alignment

**text**

A text

**annotation-table**

Table of annotations

**annotation-table-list**

A list of different tables of annotations

**ebwt-index**

 Bowtie index

**hmm2-profile**

A HMM profile of HMMER2 package

**fmatrix**

 Frequency matrix

**wmatrix**

Weight matrix

**sitecon-model**

 SITECON model

**assembly**

Assembly

**variation**

Variation track

To search an element use the name filter or press the _Ctrl+F_ shortcut that moves you to the name filter also:


![](/images/65930053/65930054.jpg)

*   [Data Readers](data-readers.md)
    *   [Read Alignment Element](read-alignment-element.md)
    *   [Read Annotations Element](read-annotations-element.md)
    *   [Read FASTQ File with SE Reads Element](read-fastq-file-with-se-reads-element.md)
    *   [Read FASTQ Files with PE Reads Element](read-fastq-files-with-pe-reads-element.md)
    *   [Read File URL(s) Element](65930060.html)
    *   [Read NGS Reads Assembly Element](read-ngs-reads-assembly-element.md)
    *   [Read Plain Text Element](read-plain-text-element.md)
    *   [Read Sequence Element](read-sequence-element.md)
    *   [Read Sequence from Remote Database Element](read-sequence-from-remote-database-element.md)
    *   [Read Variants Element](read-variants-element.md)
*   [Data Writers](data-writers.md)
    *   [Write Alignment Element](write-alignment-element.md)
    *   [Write Annotations Element](write-annotations-element.md)
    *   [Write FASTA Element](write-fasta-element.md)
    *   [Write NGS Reads Assembly Element](write-ngs-reads-assembly-element.md)
    *   [Write Plain Text Element](write-plain-text-element.md)
    *   [Write Sequence Element](write-sequence-element.md)
    *   [Write Variants Element](write-variants-element.md)
*   [Data Flow](data-flow.md)
    *   [Filter Element](filter-element.md)
    *   [Grouper Element](grouper-element.md)
    *   [Multiplexer Element](multiplexer-element.md)
    *   [Sequence Marker Element](sequence-marker-element.md)
*   [Basic Analysis](basic-analysis.md)
    *   [Amino Acid Translation Element](amino-acid-translation-element.md)
    *   [Annotate with UQL Element](annotate-with-uql-element.md)
    *   [CD-Search Element](cd-search-element.md)
    *   [Collocation Search Element](collocation-search-element.md)
    *   [Export PHRED Qualities Element](export-phred-qualities-element.md)
    *   [Fetch Sequences by ID From Annotation Element](fetch-sequences-by-id-from-annotation-element.md)
    *   [Filter Annotation by Name Element](filter-annotation-by-name-element.md)
    *   [Filter Annotations by Qualifier](filter-annotations-by-qualifier.md)
    *   [Find Correct Primer Pairs Element](find-correct-primer-pairs-element.md)
    *   [Find Pattern Element](find-pattern-element.md)
    *   [Find Repeats Element](find-repeats-element.md)
    *   [Gene-by-gene approach report](gene-by-gene-approach-report.md)
    *   [Get Sequences by Annotations Element](get-sequences-by-annotations-element.md)
    *   [Group Primer Pairs Element](group-primer-pairs-element.md)
    *   [Import PHRED Qualities Element](import-phred-qualities-element.md)
    *   [Intersect Annotations Element](intersect-annotations-element.md)
    *   [Local BLAST Search Element](local-blast-search-element.md)
    *   [Merge Annotations Element](merge-annotations-element.md)
    *   [ORF Marker Element](orf-marker-element.md)
    *   [Remote BLAST Element](remote-blast-element.md)
    *   [Sequence Quality Trimmer Element](sequence-quality-trimmer-element.md)
    *   [Smith-Waterman Search Element](smith-waterman-search-element.md)
*   [Data Converters](data-converters.md)
    *   [Convert bedGraph Files to bigWig Element](convert-bedgraph-files-to-bigwig-element.md)
    *   [Convert Text to Sequence Element](convert-text-to-sequence-element.md)
    *   [File Format Conversion Element](file-format-conversion-element.md)
    *   [Reverse Complement Element](reverse-complement-element.md)
    *   [Split Assembly into Sequences Element](split-assembly-into-sequences-element.md)
*   [DNA Assembly](dna-assembly.md)
    *   [Assembly Sequences with CAP3](assembly-sequences-with-cap3.md)
*   [HMMER2 Tools](hmmer2-tools.md)
    *   [HMM2 Build Element](hmm2-build-element.md)
    *   [HMM2 Search Element](hmm2-search-element.md)
    *   [Read HMM2 Profile Element](read-hmm2-profile-element.md)
    *   [Write HMM2 Profile Element](write-hmm2-profile-element.md)
*   [HMMER3 Tools](hmmer3-tools.md)
    *   [HMM3 Build Element](hmm3-build-element.md)
    *   [HMM3 Search Element](hmm3-search-element.md)
    *   [Read HMM3 Profile](read-hmm3-profile.md)
    *   [Write HMM3 Profile](write-hmm3-profile.md)
*   [Multiple Sequence Alignment](multiple-sequence-alignment.md)
    *   [Align Profile to Profile with MUSCLE Element](align-profile-to-profile-with-muscle-element.md)
    *   [Align with ClustalO Element](align-with-clustalo-element.md)
    *   [Align with ClustalW Element](align-with-clustalw-element.md)
    *   [Align with Kalign Element](align-with-kalign-element.md)
    *   [Align with MAFFT Element](align-with-mafft-element.md)
    *   [Align with MUSCLE Element](align-with-muscle-element.md)
    *   [Align with T-Coffee Element](align-with-t-coffee-element.md)
    *   [Extract Consensus from Alignment as Sequence](extract-consensus-from-alignment-as-sequence.md)
    *   [Extract Consensus from Alignment as Text](extract-consensus-from-alignment-as-text.md)
    *   [In Silico PCR Element](in-silico-pcr-element.md)
    *   [Join Sequences into Alignment Element](join-sequences-into-alignment-element.md)
    *   [Map to Reference Element](map-to-reference-element.md)
    *   [Split Alignment into Sequences Element](split-alignment-into-sequences-element.md)
*   [NGS: Basic Functions](65930149.html)
    *   [CASAVA FASTQ Filter Element](casava-fastq-filter-element.md)
    *   [Cut Adapter Element](cut-adapter-element.md)
    *   [Extract Consensus from Assembly Element](extract-consensus-from-assembly-element.md)
    *   [Extract Coverage from Assembly Element](extract-coverage-from-assembly-element.md)
    *   [FASTQ Merger Element](fastq-merger-element.md)
    *   [FASTQ Quality Trimmer Element](fastq-quality-trimmer-element.md)
    *   [FastQC Quality Control Element](fastqc-quality-control-element.md)
    *   [Filter BAM SAM Files Element](filter-bam-sam-files-element.md)
    *   [Genome Coverage Element](genome-coverage-element.md)
    *   [Improve Reads with Trimmomatic Element](improve-reads-with-trimmomatic-element.md)
    *   [Merge BAM Files Element](merge-bam-files-element.md)
    *   [Remove Duplicates in BAM Files Element](remove-duplicates-in-bam-files-element.md)
    *   [Slopbed Element](slopbed-element.md)
    *   [Sort BAM Files Element](sort-bam-files-element.md)
*   [NGS: Mapping Reads](65930175.html)
    *   [Assemble Reads with SPAdes Element](assemble-reads-with-spades-element.md)
    *   [Map Reads with Bowtie Element](map-reads-with-bowtie-element.md)
    *   [Map Reads with Bowtie2 Element](map-reads-with-bowtie2-element.md)
    *   [Map Reads with BWA Element](map-reads-with-bwa-element.md)
    *   [Map Reads with BWA-MEM Element](map-reads-with-bwa-mem-element.md)
    *   [Map Reads with UGENE Genome Aligner Element](map-reads-with-ugene-genome-aligner-element.md)
    *   [Map RNA-Seq Reads with TopHat Element](map-rna-seq-reads-with-tophat-element.md)
*   [NGS: RNA-Seq Analysis](65930197.html)
    *   [Assemble Transcripts with StringTie Element](assemble-transcripts-with-stringtie-element.md)
    *   [Assembly Transcripts with Cufflinks Element](assembly-transcripts-with-cufflinks-element.md)
    *   [Extract Transcript Sequences with gffread Element](extract-transcript-sequences-with-gffread-element.md)
    *   [Merge Assemblies with Cuffmerge Element](merge-assemblies-with-cuffmerge-element.md)
    *   [StringTie Gene Abudance Report Element](stringtie-gene-abudance-report-element.md)
    *   [Test for Diff. Expression with Cuffdiff Element](Test-for-Diff.expression-with-cuffdiff-element.md)
*   [NGS: Variant Analysis](65930204.html)
    *   [Call Variants with SAMtools Element](call-variants-with-samtools-element.md)
    *   [Change Chromosome Notation for VCF Element](change-chromosome-notation-for-vcf-element.md)
    *   [Convert SnpEff Variations to Annotations Element](convert-snpeff-variations-to-annotations-element.md)
    *   [Create VCF Consensus Element](create-vcf-consensus-element.md)
    *   [SnpEff Annotation and Filtration Element](snpeff-annotation-and-filtration-element.md)
*   [Transcription Factor](transcription-factor.md)
    *   [Build Frequency Matrix Element](build-frequency-matrix-element.md)
    *   [Build SITECON Model Element](build-sitecon-model-element.md)
    *   [Build Weight Matrix Element](build-weight-matrix-element.md)
    *   [Convert Frequency Matrix Element](convert-frequency-matrix-element.md)
    *   [Read Frequency Matrix Element](read-frequency-matrix-element.md)
    *   [Read SITECON Model Element](read-sitecon-model-element.md)
    *   [Read Weight Matrix Element](read-weight-matrix-element.md)
    *   [Search for TFBS with SITECON Element](search-for-tfbs-with-sitecon-element.md)
    *   [Search for TFBS with Weight Matrix Element](search-for-tfbs-with-weight-matrix-element.md)
    *   [Write Frequency Matrix Element](write-frequency-matrix-element.md)
    *   [Write SITECON Model Element](write-sitecon-model-element.md)
    *   [Write Weight Matrix Element](write-weight-matrix-element.md)
*   [Utils](utils.md)
    *   [DNA Statistics Element](dna-statistics-element.md)
    *   [Generate DNA Element](generate-dna-element.md)


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
