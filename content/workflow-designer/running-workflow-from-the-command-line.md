---
title: "Running Workflow from the Command Line"
weight: 900
---


# Running Workflow from the Command Line

UGENE provides command line interface (CLI). To learn more about UGENE CLI and commands available read [main UGENE User Manual](http://ugene.unipro.ru/documentation.html).

This chapter describes how you can create a new command using a _workflow_.

To run a workflow from the command line do the following:

*   Create the workflow in the Workflow Designer. For example on the image below the _Align sequences with MUSCLE_ sample workflow is used:

![](/images/2097213/2359337.png)

*   Now you should configure aliases for those parameters and ports and slots that you are going to use from the command line. To do it select the _Actions ‣ Set parameter aliases..._ item in the main menu or the _Set parameter aliases_ toolbar button. The following dialog appears:

![](/images/65930020/65930021.png)

It contains the list of objects that corresponds to the _elements_ of the workflow. For each object the list of parameters is available for which you can assign command line aliases. For example, assign alias **in** to parameter _Input file_ (of the _Read alignment_ element):

![](/images/65930020/65930022.png)

And alias **out** to parameter _Output file_ (of the _Write Stockholm_ element).

![](/images/65930020/65930023.png)

To select ports and slots aliases use the following dialog by the _Actions->Configure port and slot aliases_ main menu item:

![](/images/65930020/65930024.png)

Press the _Ok_ button to save aliases and close the dialog. When you create aliases you can import workflow to element by the _Actions->Import workflow to element_ main menu item.

*   [_Save the workflow_](manipulating-workflow/saving-workflow) to a file: if you follow the example, choose the _Actions ‣ Save workflow as..._ item in the main menu, browse for the file location and enter **mySchema** as the workflow name. This name will be used to launch the workflow from the command line.
*   Launch the workflow from the command line:


\[path\_to\_ugene\\\]ugene --task={schema\_name} \[--{parameter1}={value1} \[--{parameter2}={value2} ...\]\]

The run information will be saved into the text file. By default it is the working directory.

For example on Windows the command can look as follows:

ugene --task=C:\\mySchema --in=C:\\COI.aln --out=C:\\COI.sto

In this example the path to the directory with the UGENE executable is added to the system PATH variable.
