---
title: "Workflow Elements and Connections"
weight: 300
---

# Workflow Elements and Connections

The [_Scene_](workflow-designer-window-components) is initially empty, and you start by creating a workflow on it:

**Workflow**

A workflow is a visual representation of the data flow. It consists of workflow elements and their connections.

**Workflow Element**

An element of a workflow. Different elements are used to read data from files on disk, perform some algorithms, and write data to files on disk. Each element contains one or several input and output ports.

**Element Connection**

A connection between two elements specifies that data in the output port of one element should be passed to a matching input port of another element.

**Input Port**

An input port of an element is used to collect data from another element. A workflow element may have several input ports. On the Scene, such a port is displayed as a right semicircle.

**Output Port**

An output port of an element is used to provide data to another element. A workflow element may have one output port or none. On the Scene, the port is displayed as a left semicircle.

**Slot**

Each port has one or several slots. A slot is the smallest passageway to transfer the workflow data through. It has a specific type (e.g., "Sequence", "Set of annotations", etc.). For example, only sequence data can be passed through a sequence slot.

Thus, an input port has one or several **input slots**. These slots specify data that are expected as input by the element. An output port has one or several **output slots**. These slots specify the data that the element produces.

In a workflow, an element usually has access to slots of the connected elements located earlier in the workflow.

**Message**

A message is a single data chunk, transferred from an output slot of one element to an input slot of another element. The slots must have the same type to make the transfer possible.

The Scene is initially empty, and you start by creating a workflow on it:

See an example of a workflow in the image below:

![](/images/1474798/2359298.png)

Your first step is to [_add_](../manipulating-element/adding-element) the necessary workflow elements, for example, by dragging them from the [_Palette_](workflow-designer-window-components) to the Scene[:](http://ugene.unipro.ru/documentation/wd_manual/introduction/wd_window_components.html#term-scene)

![](/images/1474798/2359300.png)

The added element can be moved around on the Scene by dragging it and can be resized by dragging its borders. Read the chapter [_Manipulating Element_](manipulating-element.md) to learn what else you can do with workflow elements.

If you have two elements with matching output and input ports, you can make the connection by dragging the arrow between the ports:

![](/images/1474798/2359301.png)

All matching ports of available processes are highlighted while you drag the arrow, and the arrow sticks to a near match as you drag closer. If an element has a single matching port, you can simply drop the arrow on the element itself to create a correct connection.

Once created, a connection will follow the movements of the linked elements; you cannot redirect or reshape the connection arrow but only remove it. You can move the port around the element to which it belongs by dragging it while holding the Alt key. This is helpful for fine-tuning the visual layout of a workflow.