---
title: "Importing Annotations from CSV"
weight: 1000
---

# Importing Annotations from CSV

It is possible to import annotations for a sequence from an annotations table stored in CSV format.

To import annotations from a CSV file, right-click on a _Project View_ and select _Import ‣ Import annotations from CSV_. The following dialog box will appear:

![](/images/65929493/65929494.png)

You need to specify the file from which to read the annotations table _(required)_:

![](/images/65929493/65929495.png)

And specify the format of and the path to the file into which to write the annotations table _(required)_:

![](/images/65929493/65929496.png)

Check _Add result file to project_ to link the annotations to the currently opened sequence.

![](/images/65929493/65929497.png)

To use a separator for splitting the table, check the _Column separator_ item and specify the separator symbols. You can also press _Guess_ to attempt to detect the separator from the input file.

![](/images/65929493/65929498.png)

Alternatively, you can press _Edit_ to modify the script that specifies the separator for each parsed line. It is possible to use the line number in the script.

![](/images/65929493/65929499.png)

Using the arrows, you can exclude the necessary number of lines at the beginning of the document from parsing. You can also skip all lines that start with the specified text.

![](/images/65929493/65929500.png)

By pressing _Preview_, you can view the current annotations table (produced from the input file with the specified parameter values). The input file contents will also be shown at the bottom part of the dialog.

![](/images/65929493/65929501.png)

The preview table headline indicates the types of information contained in the corresponding columns. By default, the values are _\[ignored\]_. To specify a column role, click on the corresponding headline element:

![](/images/65929493/65929502.png)

The annotation start and end positions must be specified. It is possible to add an offset to every read start position by checking the _Add offset_ checkbox, and to shorten annotations by one from the end by unchecking the _Inclusive_ checkbox.

When all the roles are specified, press _Run_. With the _Add to project_ checkbox checked and a _Sequence View_ opened, if successful, you will see the _Sequence View_ with annotations linked:

![](/images/65929493/65929503.png)