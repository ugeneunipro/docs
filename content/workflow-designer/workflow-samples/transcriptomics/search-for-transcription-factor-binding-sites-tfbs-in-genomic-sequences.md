---
title: "Search for Transcription Factor Binding Sites (TFBS) in Genomic Sequences"
weight: 1
---


# Search for Transcription Factor Binding Sites (TFBS) in Genomic Sequences

This workflow predicts binding sites for number of transcription factors of interest using SITECON algorithm. The present workflow sample is designed for simultaneous recognition of binding sites for 3 different transcription factor types, you can expand it for recognition of any desired number of transription factor types.SITECON - is a program pakage for recognition of potential transcription factor binding sites basing on the data about conservative conformational and physicochemical properties revealed on the basis of the binding sites sets analysis.Citing SITECON Please cite:Oshchepkov D.Y., Vityaev E.E., Grigorovich D.A., Ignatieva E.V., Khlebodarova T.M.SITECON:a tool for detecting conservative conformational and physicochemicalproperties in transcription factor binding site alignments and for siterecognition. // Nucleic Acids Res. 2004 Jul 1;32(Web Server issue):W208-12.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](how-to-use-sample-workflows.md)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Search for Transcription Factor Binding Sites (TFBS) in Genomic Sequences" can be found in the "Transcriptomics" section of the Workflow Designer samples.

##### Workflow Image

The workflow looks as follows:


![](/images/65930593/65930594.png)

##### Workflow Wizard

The wizard has 5 pages.

1.  Input sequence(s): On this page you must input sequence(s).


    ![](/images/65930593/65930595.png)

2.  Search for TFBS 1, 2, 3: On these pages you can modify search for TFBS parameters.


    ![](/images/65930593/65930596.png)

    The following parameters are available:

    Input file(s)

    Semicolon-separated list of paths to the input files.

    Result annotation

    Annotation name for marking found regions.

    Search in

    Which strands should be searched: direct, complement or both.

    Min score

    Recognition quality percentage threshold.

    If you need to switch off this filter choose the lowest value

    Min Err 1

    Alternative setting for filtering results, minimal value of Error type I.
    Note that all thresholds (by score, by err1 and by err2) are applied when filtering results.

    If you need to switch off this filter choose "0" value

    Max Err 2

    Alternative setting for filtering results, max value of Error type II.
    Note that all thresholds (by score, by err1 and by err2) are applied when filtering results.

    If you need to switch off this filter choose "1" value

3.  Output data: On this page you can modify output parameters.


    ![](/images/65930593/65930597.png)
