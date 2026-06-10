---
title: "Pattern Algorithm Element"
weight: 900
---

# Pattern Algorithm Element

The _element_ searches for the specified pattern in the provided sequence.

Parameters in GUI
-----------------

| Parameter    | Description                        | Default value      |
|--------------|------------------------------------|--------------------|
| **Annotate As** | Name of the result annotations.   | misc\_feature       |
| **Pattern**  | The pattern to search for.         | You must specify a value! |
| **Direction**| See the description [_here_](/query-designer/manipulating-schema/managing-strands/element-direction-in-schema/). | Any                |

Parameters in Schema File
-------------------------

**Type:** search

| Parameter     | Parameter in the GUI | Type   |
|---------------|----------------------|--------|
| **key**       | **Annotate As**      | _string_ |
| **pattern**   | **Pattern**          | _string_ |