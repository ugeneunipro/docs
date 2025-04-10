---
title: "Data Analysis Tools"
weight: 500
---

# Data Analysis Tools

UGENE provides a graphical user interface (GUI) for a variety of bioinformatics tools. A tool is supplied either as embedded or external:

* **Embedded tool:** The tool is integrated into the UGENE source code. Such tools are always available in UGENE, independent of the UGENE package type and operating system.
* **External tool:**
    * **Integrated (supported) external tool:** The tool's executable file(s) is provided with UGENE. It is launched when used in the UGENE GUI, and the results are also displayed within the UGENE GUI. Note that the tool may only be available on some operating systems.
    * **Custom external tool:** It is possible to add [any custom external tool](https://local.ugene.unipro.ru/wiki/display/WDD33/Custom+Elements+with+External+Tools) as a workflow element in the Workflow Designer. See the "[Custom External Tools](../basic-functions/ugene-application-settings/external-tools/custom-external-tools)" documentation chapter for details.

### Specify Integrated External Tools in the Installed Package

Most external tools (if available on the target operating system) are installed by default with the Online Installer.

You can specify the tools manually:

1. Download the tool executables from the links on the web page [http://ugene.net/download-all.html](http://ugene.net/download-all.html):
   * **External Tools Package:** This package contains all external tools except JRE (i.e., "java") and RScript.
   * **Java Runtime Environment (JRE):** Although UGENE is not a Java application, a few tools (e.g., FastQC, Trimmomatic) require JRE. Make sure [JRE 8](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) or higher is installed.
   * **RScript:** R is currently used in UGENE for ChIP-Seq data analysis only.

2. Configure the tools in UGENE: [Open the UGENE Application Settings](ugene-application-settings.md) dialog, select the "[External Tools](external-tools.md)" page, and specify the external tool executables.

### Integrated External Tools

See the table below for the list of currently integrated external tools, information about their availability on different operating systems, and the version included in the corresponding External Tools Package.

| External Tool                     |                           | Windows (64-bit)                                    | macOS (64-bit)           | Linux (64-bit)           |
|-----------------------------------|---------------------------|-----------------------------------------------------|--------------------------|--------------------------|
| bigwig                            |                           | 4                                                   | 4                        | 4                        |
| bedtools                          |                           | 2.29.2                                              | 2.31.0                   | 2.31.0                   |
| BLAST                             |                           | 2.14.0                                              | 2.12.0                   | 2.14.0                   |
| Bowtie                            |                           | 1.3.0                                               | 1.3.0                    | 1.3.0                    |
| Bowtie2                           |                           | 2.4.2                                               | 2.4.2                    | 2.4.2                    |
| BWA                               |                           | 0.7.17-r1188                                        | 0.7.17-r1188             | 0.7.17-r1188             |
| CAP3                              |                           | 12/21/07                                            | 12/21/07                 | 10/15/07                 |
| Cistrome  <br>(until UGENE v.41)  | CEAS Tools (need Rscript) | 0.9.9.7                                             | 0.9.9.7                  | 0.9.9.7                  |
| conservation\_plot (need Rscript) |                           | 0.1                                                 | 0.1                      | 0.1                      |
| go\_analysis (need Rscript)       |                           | 1.0.1                                               | 1.0.1                    | 1.0.1                    |
| MACS                              |                           | 1.4.2                                               | 1.4.2                    | 1.4.2                    |
| peak2gene                         |                           | 1.02                                                | 1.02                     | 1.02                     |
| seqpos (need Rscript)             |                           | 2.0                                                 | 2.0                      | 2.0                      |
| CLARK (until UGENE v.40)          |                           | N/A                                                 | 1.2.4 (UGENE-customized) | 1.2.4 (UGENE-customized) |
| ClustalO                          |                           | 1.2.2                                               | 1.2.3                    | 1.2.4                    |
| ClustalW                          |                           | 2.1                                                 | 2.1                      | 2.1                      |
| Cufflinks                         |                           | N/A                                                 | 2.2.1                    | 2.2.1                    |
| cutadapt (until UGENE v.49)       |                           | 1.7.1                                               | 1.7.1                    | 1.7.1                    |
| DIAMOND (until UGENE v.40)        |                           | N/A                                                 | 0.9.22                   | 0.9.22                   |
| FastQC                            |                           | 0.12.1                                              | 0.12.1                   | 0.12.1                   |
| FastTree (since UGENE v.46)       |                           | 2.1.11                                              | 2.1.11                   | 2.1.11                   |
| HMMER                             |                           | 3.3.1                                               | 3.3.1                    | 3.3.1                    |
| IQ-TREE (since UGENE v.41)        |                           | 1.6.12                                              | 1.6.12                   | 1.6.12                   |
| JRE (java)                        |                           | 1.8.0\_192                                          | 1.8.0\_192               | 11.0.11                  |
| Kalign                            |                           | 3.3.5                                               | 3.3.5                    | 3.3.5                    |
| Kraken (until UGENE v.40)         |                           | N/A                                                 | 1.0                      | 1.0                      |
| MAFFT                             |                           | 7.520                                               | 7.520                    | 7.520                    |
| MetaPhlAn2 (until UGENE v.40)     |                           | N/A                                                 | 2.7.7                    | 2.0.0                    |
| mfold (since UGENE v.50)          |                           | 3.6                                                 | 3.6                      | 3.6                      |
| MrBayes                           |                           | 3.2.3                                               | 3.2.3                    | 3.2.3                    |
| Perl                              |                           | 5.24.3                                              | N/A                      | N/A                      |
| PhyML Maximum Likelihood          |                           | 3.3.20220408                                        | 3.3.20220408             | 3.3.20220408             |
| Python3                           |                           | 3.12.1                                              | N/A                      | 3.12.1                   |
| Cutadapt                          |                           | 4.6                                                 | N/A                      | 4.6                      |
| Rscript                           |                           | R is not included in the External Tools Packages.   |                          |                          |
| SAMtools                          |                           | 0.1.19                                              | 0.1.19                   | 0.1.19                   |
| Tabix                             |                           | 0.2.5                                               | 0.2.6                    | 0.2.6                    |
| vcfutils                          |                           | Version not specified                               | Version not specified    | Version not specified    |
| SnpEff                            |                           | 4.3i                                                | 4.3i                     | 4.3i                     |
| SPAdes                            |                           | N/A                                                 | 3.15.5                   | 3.15.5                   |
| Spidey                            |                           | 1.0                                                 | N/A                      | 1.0                      |
| StringTie                         |                           | N/A                                                 | 1.3.4d                   | 1.3.6                    |
| TopHat                            |                           | N/A                                                 | 2.1.1                    | 2.1.1                    |
| Trimmomatic                       |                           | 0.39                                                | 0.39                     | 0.39                     |
| vcf-consensus                     |                           | 0.1.16                                              | 0.1.16                   | 0.1.16                   |
| WEVOTE (until UGENE v.40)         |                           | N/A                                                 | 1.0                      | 1.0                      |