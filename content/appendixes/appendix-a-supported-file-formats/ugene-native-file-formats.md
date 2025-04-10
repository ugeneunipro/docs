---
title: "UGENE Native File Formats"
weight: 200
---

# UGENE Native File Formats

| File Format                       | File Extension               | Read | Write | Comment                                                                                       |
|-----------------------------------|------------------------------|------|-------|-----------------------------------------------------------------------------------------------|
| **Dotplot**                       | \*.dpt                       | +    | +     | Stores a dotplot of a sequence.                                                               |
|                                   |                              |      |       | **See also:** [_Dotplot_](dotplot.md)                                                         |
| **UGENE database file**           | \*.ugenedb                   | +    | +     | UGENE database files store information for imported BAM or SAM files and can be used for converting this information into a SAM file. |
|                                   |                              |      |       | **See also:** [_Import BAM/SAM File_](../../assembly-browser/import-bam-and-sam-files)        |
| **Short Reads FASTA**             | \*.srfa, \*.srfasta          | +    | +     | A multiple sequence alignment file format.                                                    |
|                                   |                              |      |       | **See also:** [_Alignment Editor_](alignment-editor.md)                                       |
| **UGENE Workflow Language**       | \*.uwl                       | +    | +     | Human-readable format to store workflows created in the UGENE _Workflow Designer_.            |
|                                   |                              |      |       | **See also:** [_Workflow Designer_](workflow-designer.md)                                     |
| **UGENE Query Language**          | \*.uql                       | +    | +     | Human-readable format to store schemas created in the UGENE _Query Designer_.                 |
|                                   |                              |      |       | **See also:** [_Query Designer_](https://local.ugene.unipro.ru/wiki/display/QDD34/Query+Designer+Documentation) |
| **Workflow element for command line tool** | \*.etc             | +    | +     | Format for storing workflow elements that can launch an external command line tool.           |
|                                   |                              |      |       | **See also:** [_Workflow Designer_](workflow-designer.md)                                     |