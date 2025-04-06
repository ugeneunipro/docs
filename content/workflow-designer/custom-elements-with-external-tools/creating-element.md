---
title: "Creating Element"
weight: 1
---


# Creating Element

To create an element for a command line tool select either _Actions ‣ Create element with external tool_ in the main menu or the following icon on the toolbar:


![](/images/2097199/2359321.png)

The _Configure Element with External Tool_ wizard appears. On the first page of the wizard input a name and external command-line tool. Letters, numbers and underscores are allowed in the name.


![](/images/65929990/65929991.jpg)

On the second page add the required input data:


![](/images/65929990/65929992.jpg)

On the third page of the wizard you can add parameters for the command line tool. Later you would be able to set values for the parameters in the Property Editor.


![](/images/65929990/65929993.jpg)

On the next page add the required output data:


![](/images/65929990/65929994.jpg)

For each input or output you should:

*   Input a name (letters, numbers, and underscores are allowed in the name).
*   Select a type: multiple alignment, sequence, sequence with annotations, a set of annotations or string.
*   Optionally input a description.

For each parameter added you should:

*   Input a name (letters, numbers and underscores are allowed in the name).
*   Select its type: boolean, number, string or URL.
*   Optionally input the description.

On the next page of the wizard you should input the execution string, i.e. the command that would be executed.


![](/images/65929990/65929995.png)

The signature of the execution string depends on the command that is launched. But the general rule is that input/output data and attributes have prefix $. You can set the parameterized description for the new element (the description that appears not in property editor but on the element itself). In the parameterized description, you also can use parameters substitution with prefix $. If the paths in the execution string contain spaces, they must be enclosed with quotes.

On the next wizard page, you can optionally input the description of the element. It would be shown on the element on the [_Scene_](http://ugene.unipro.ru/documentation/wd_manual/introduction/wd_window_components.html#term-scene). The description can be parameterized. This means that if you input e.g. an attribute name (with prefix $), the name on the element would be substituted with the value of the corresponding parameter. For example input the following parameters:


![](/images/65929990/65929996.jpg)

On the next wizard page, you can see the final element summary:


![](/images/65929990/65929997.jpg)

The created element is added to the Workflow Designer scene, and can be connected with other elements in a workflow:


![](/images/65929990/65929998.png)

The new element also becomes available in the "Custom Elements with External Tools" group on the "Elements" tab of the Workflow Designer palette (at the left part of the window), so that you can use it at any time in other workflow.
