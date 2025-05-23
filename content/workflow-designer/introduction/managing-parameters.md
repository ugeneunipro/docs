---
title: "Managing Parameters"
weight: 400
---

# Managing Parameters

When you select an [_element_](workflow-elements-and-connections) on the [_Scene_](workflow-designer-window-components), the [_Property Editor_](workflow-designer-window-components) displays detailed information about it: its name, description, parameters, [_input_](workflow-elements-and-connections) and [_output_](workflow-elements-and-connections) ports, etc. To change the name of the element displayed on the Scene, edit the _Element name_ value.

All the parameters available for the element are displayed in the _Parameters_ area. Some parameters must have a value, and they are displayed in bold. Notice that when you select a parameter, its description is shown below. To modify a value, click on it. Depending on the parameter’s type, you may be required to either input a value or browse for a file(s). Additionally, you can configure slots of a connected input port by selecting different (matching) data available through the dataflow. More advanced users can use their own scripts to set a parameter’s value; read chapter [_Using Script to Set Parameter Value_](../using-script-to-set-parameter-value) to learn more. The image below shows the _Property Editor_:

![](/images/65929883/65929884.jpg)

For _[Data Readers](data-readers.md)_, you can manipulate files or directories with the help of datasets:

![](/images/65929883/65929885.png)

To remove files from a dataset, you can select it and press the _Delete_ button.

For [Data Writers](data-writers.md), if the _Output file_ parameter is empty, UGENE will generate output file names automatically. You can use the _Output file suffix_ parameter to manipulate it.