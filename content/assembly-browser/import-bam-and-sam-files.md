---
title: "Import BAM and SAM Files"
weight: 100
---

# Import BAM and SAM Files

To begin working with an assembly, import it into the UGENE database file. To do this, [_open_](opening-document.md) the assembly file.

For assembly files without a header, you can select a file with the reference sequence; otherwise, the header information will be generated automatically.

![](/images/65929794/65929795.png)

Select if you want the reference sequence and click the _Import_ button.

For other assembly files, the following dialog appears:

![](/images/65929794/65929796.png)

The _Source URL_ field in the dialog specifies the file to import. The _Info_ button nearby can be used to obtain additional information about the file.

There is a list of contigs below the _Source URL_. Check the contigs that you want to import into the database. You can use the _Select All_, _Deselect All_, and _Invert Selection_ buttons to manage the selection.

The _Destination URL_ field specifies the output database file.

If you check _Import unmapped reads_, then all unmapped reads in the assembly (i.e., reads with the unmapped flag or without CIGAR) are imported. Note, however, that they are not visualized in the current UGENE version.

To start the import, click the _Import_ button in the dialog. You can see the progress of the import in the [_Task View_](http://ugene.unipro.ru/documentation/manual/basic_functions/ugene_terminology.html#term-task-view). To export a UGENE database file into the SAM format, select the _Actions ‣ Export assembly to SAM format_ item in the main menu.