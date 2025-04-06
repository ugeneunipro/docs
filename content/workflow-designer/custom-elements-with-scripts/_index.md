---
title: "Custom Elements with Scripts"
weight: 1
---


# Custom Elements with Scripts

It is possible to create custom algorithmic blocks using scripts in the Workflow Designer.

To create an element either select _Actions ‣ Create  Element with Script_ in the main menu.

The _Create Element with Script_ dialog will appear:


![](/images/65929977/65929978.png)

Here you should set the name of the element, its description and input/output ports of the element. It is possible to create a port with several input/output slots.

There are 4 types of data for a slot available:

*   Multiple alignments
*   Sequence
*   Set of annotations
*   Files

You can also add an attribute. The following types are supported for attributes:

*   String
*   Number
*   Boolean

The element created is stored in a directory that can be set in the [_Application Settings_](application-settings.md) dialog.

The element also becomes available in the _Custom Elements with Scripts_ group on the [_Palette_](workflow-designer-window-components.md).

It is required to write a script for the element. Supported languages for the script are languages based on the ECMAScript (Javascript, QtScript).

To edit the script select the element on the _Scene_ and either select _Actions ‣ Edit script of the element_ in the main menu or use the _Edit script of the element_ item in the context menu.

The _Script editor_ dialog will appear:


![](/images/65929977/65929979.png)

As you can see there are predefined variables for the ports and the attributes in the script. The variables for the input slots begin with the “in\_” prefix, variables for the output slots begin with the “out\_” prefix. It is possible to load a script from a file (use the _Used script_ field to do it).

For each supported data type UGENE provides a number of functions that can be used in the scripts.

*   [Functions Supported for Multiple Alignment Data](functions-supported-for-multiple-alignment-data.md)
*   [Functions Supported for Sequence Data](functions-supported-for-sequence-data.md)
*   [Functions Supported for Set of Annotations Data](functions-supported-for-set-of-annotations-data.md)
*   [Functions Supported for Files](functions-supported-for-files.md)
*   [Common Function](common-function.md)


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
