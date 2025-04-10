---
title: "Assembly Browser"
weight: 1000
---

# Assembly Browser

The UGENE Assembly Browser project, which began in 2010, was inspired by the [Illumina iDEA Challenge 2011](https://archive.is/20130126033841/http://www.illumina.com/idea) and numerous requests from UGENE users. The main objective of the Assembly Browser is to enable users to visualize and efficiently navigate large next-generation sequence assemblies.

Currently supported formats are SAM (Sequence Alignment/Map) and BAM, which is the binary version of the SAM format. Both formats are produced by SAMtools and are described in the following specification: [SAMtools](http://samtools.sourceforge.net/SAM1.pdf). Support for other formats is also planned, so please send us a request if you are interested in a particular format.

To browse assembly data in UGENE, a BAM or SAM file should be imported into a UGENE database file. After that, you can convert the UGENE database file into a SAM file. Importing to a UGENE database file has both advantages and disadvantages. The disadvantages include the potential time required for importing a large file and the need for sufficient disk space to store the database file.

On the other hand, this allows users to overview the entire assembly and navigate through it relatively quickly. Additionally, during the import process, you can select specific contigs to be imported from the BAM/SAM file. Thus, there is no need to import the entire file if you plan to work only with certain contigs. Note that in the future, there are plans to support an alternative approach, specifically when a BAM/SAM file is opened directly.

The Assembly Browser has been tested on various BAM/SAM files from the [1000 Genomes Project](http://www.1000genomes.org/about) as well as from other sources.

Read the documentation below to learn more about the features of the Assembly Browser.