---
title: "Importing Annotations from CSV"
weight: 1
---


# Importing Annotations from CSV

It is possible to import annotations for a sequence from an annotations table stored in the CSV format.

To import annotations from a CSV file, right-click on a _Project View_ and select _Import ‣ Import annotations from CSV_. The following dialog box will appear:


![](/images/65929493/65929494.png)

Basically you need to specify the file to read annotations table from _(required)_:


![](/images/65929493/65929495.png)

And the format of and the path to the file to write the annotations table into _(required)_:


![](/images/65929493/65929496.png)

Check _Add result file to project_ to link the annotations to the currently opened sequence.


![](/images/65929493/65929497.png)

To use a separator to split the table, check the _Column separator_ item and specify the separator symbols. Also you can press _Guess_ to try to detect the separator from the input file.


![](/images/65929493/65929498.png)

Alternatively, you can press _Edit_ and edit the script which will specify the separator for each parsed line. It is possible to use line number in the script.


![](/images/65929493/65929499.png)

Using the arrows, you exclude the necessary number of lines at the beginning of the document from parsing. You can also skip all lines that start with the specified text.


![](/images/65929493/65929500.png)

By pressing _Preview_ one can bring up the view of the current annotations table (which is produced from the input file with the specified parameters values). The input file contents will also be shown at the bottom part of the dialog.


![](/images/65929493/65929501.png)

The preview table headline indicates the types of the information contained in the corresponding columns. By default the values are _\[ignored\]_. To specify a column role, click on the corresponding headline element:


![](/images/65929493/65929502.png)

The annotation start and end positions must be specified. It is possible to add an offset to every read start position by checking the _Add offset_ checkbox, and to shorten annotations by one from the end by uncheking the _Inclusive_ checkbox.

When all the roles are specified, press _Run_. With the _Add to project_ checkbox specified and a _Sequence View_ opened, on success you will see the _Sequence View_ with annotations linked:


![](/images/65929493/65929503.png)
