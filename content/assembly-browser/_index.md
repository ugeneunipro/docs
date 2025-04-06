---
title: "Assembly Browser"
weight: 1
---


# Assembly Browser

The UGENE Assembly Browser project started in 2010 was inspired by [Illumina iDEA Challenge 2011](https://archive.is/20130126033841/http://www.illumina.com/idea) and multiple requests from UGENE users. The main goal of the Assembly Browser is to let a user visualize and efficiently browse large next generation sequence assemblies.

Currently supported formats are SAM (Sequence Alignment/Map) and BAM, which is a binary version of the SAM format. Both formats are produced by SAMtools and described in the following specification: [SAMtools](http://samtools.sourceforge.net/SAM1.pdf). Support of other formats is also planned, so please send us a request if you’re interested in a certain format.

To browse an assembly data in UGENE, a BAM or SAM file should be imported to a UGENE database file. After that you can convert the UGENE database file into a SAM file. The import to a UGENE database file has both advantages and disadvantages. The disadvantages are that the import may take time for a large file and there should be enough disk space to store the database file.

On the other hand, this allows one to overview the whole assembly and navigate in it rather rapidly. In addition, during the import you can select contigs to be imported from the BAM/SAM file. So, there is no need to import the whole file if you’re going to work only with some contigs. Note that in the future there are plans to support the other approach as well, namely, when a BAM/SAM file is opened directly.

The Assembly Browser has been tested on different BAM/SAM files from the [1000 Genomes Project](http://www.1000genomes.org/about) and other sources.

Read the documentation below to learn more about the Assembly Browser features.

*   [Import BAM and SAM Files](import-bam-and-sam-files.md)
*   [Browsing and Zooming Assembly](browsing-and-zooming-assembly.md)
    *   [Opening Assembly Browser Window](opening-assembly-browser-window.md)
    *   [Assembly Browser Window](assembly-browser-window.md)
    *   [Assembly Browser Window Components](assembly-browser-window-components.md)
    *   [Reads Area Description](reads-area-description.md)
    *   [Assembly Overview Description](assembly-overview-description.md)
    *   [Ruler and Coverage Graph Description](ruler-and-coverage-graph-description.md)
    *   [Go to Position in Assembly](go-to-position-in-assembly.md)
    *   [Using Bookmarks for Navigation in Assembly Data](using-bookmarks-for-navigation-in-assembly-data.md)
*   [Getting Information About Read](getting-information-about-read.md)
*   [Short Reads Vizualization](short-reads-vizualization.md)
    *   [Reads Highlighting](reads-highlighting.md)
    *   [Reads Shadowing](reads-shadowing.md)
*   [Associating Reference Sequence](associating-reference-sequence.md)
*   [Associating Variations](associating-variations.md)
*   [Consensus Sequence](consensus-sequence.md)
*   [Exporting](exporting.md)
    *   [Exporting Reads](exporting-reads.md)
    *   [Exporting Visible Reads](exporting-visible-reads.md)
    *   [Exporting Coverage](exporting-coverage.md)
    *   [Exporting Consensus](exporting-consensus.md)
    *   [Exporting Consensus Variations](exporting-consensus-variations.md)
    *   [Exporting Assembly as Image](exporting-assembly-as-image.md)
    *   [Exporting Assembly Region](exporting-assembly-region.md)
*   [Options Panel in Assembly Browser](options-panel-in-assembly-browser.md)
    *   [Navigation in Assembly Browser](navigation-in-assembly-browser.md)
    *   [Assembly Statistics](assembly-statistics.md)
    *   [Assembly Browser Settings](assembly-browser-settings.md)
*   [Assembly Browser Hotkeys](assembly-browser-hotkeys.md)
    *   [Assembly Overview Hotkeys](assembly-overview-hotkeys.md)
    *   [Reads Area Hotkeys](reads-area-hotkeys.md)


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
