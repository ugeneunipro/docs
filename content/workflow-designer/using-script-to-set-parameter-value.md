---
title: "Using Script to Set Parameter Value"
weight: 800
---


# Using Script to Set Parameter Value

When you select an element the _Parameters_ area of the [_Property Editor_](workflow-designer-window-components.md) displays two columns: _Name_ and _Value_.

Select the _Show scripting options_ item in the _Scripting mode_ menu on the toolbar or in the _Actions_ main menu.

![](/images/2097207/2359330.png)

You can see that the third column _Script_ has appeared in the _Parameters_ area, for example:

![](/images/2097207/2359331.png)

A script value can either be:

*   not available for a parameter (_N/A_ value)
*   not set (_no script_)
*   set by user (_user script_)

To set a script value (when it is available) select the _user script_ item in the _Script_ column. The following dialog appears:

![](/images/65930015/65930016.png)

Here you can see the variables available from the dataflow and can write your script. Supported languages for the script are languages based on the ECMAScript (Javascript, QtScript).
