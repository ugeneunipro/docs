---
title: "Assembly Browser"
weight: 1000
---


# Assembly Browser

The UGENE Assembly Browser project started in 2010 was inspired by [Illumina iDEA Challenge 2011](https://archive.is/20130126033841/http://www.illumina.com/idea) and multiple requests from UGENE users. The main goal of the Assembly Browser is to let a user visualize and efficiently browse large next generation sequence assemblies.

Currently supported formats are SAM (Sequence Alignment/Map) and BAM, which is a binary version of the SAM format. Both formats are produced by SAMtools and described in the following specification: [SAMtools](http://samtools.sourceforge.net/SAM1.pdf). Support of other formats is also planned, so please send us a request if you’re interested in a certain format.

To browse an assembly data in UGENE, a BAM or SAM file should be imported to a UGENE database file. After that you can convert the UGENE database file into a SAM file. The import to a UGENE database file has both advantages and disadvantages. The disadvantages are that the import may take time for a large file and there should be enough disk space to store the database file.

On the other hand, this allows one to overview the whole assembly and navigate in it rather rapidly. In addition, during the import you can select contigs to be imported from the BAM/SAM file. So, there is no need to import the whole file if you’re going to work only with some contigs. Note that in the future there are plans to support the other approach as well, namely, when a BAM/SAM file is opened directly.

The Assembly Browser has been tested on different BAM/SAM files from the [1000 Genomes Project](http://www.1000genomes.org/about) and other sources.

Read the documentation below to learn more about the Assembly Browser features.
