---
title: "Restriction Sites Algorithm Element"
weight: 800
---

# Restriction Sites Algorithm Element

The _element_ searches for restriction sites in the input sequence.

Parameters in GUI
-----------------

| Parameter     | Description                                                                                                                | Default value                             |
|---------------|----------------------------------------------------------------------------------------------------------------------------|-------------------------------------------|
| **Annotate As** | Name of the result annotations. Special value <rsite> is used. It specifies to use the enzyme names as names of the result annotations. |                                           |
| **Circular**   | If _True_, allows searching for restriction sites between the end and the beginning of the sequence.                       | False                                     |
| **Enzymes**    | Restriction enzymes used to recognize the restriction sites. You must specify a value!                                     |                                           |

Parameters in Schema File
-------------------------

| **Type:** rsite | Parameter       | Parameter in the GUI | Type     |
|-----------------|-----------------|----------------------|----------|
| **key**         | **Annotate As** |                      | _string_ |
| **circular**    | **Circular**    |                      | _boolean_|
| **enzymes**     | **Enzymes**     |                      | _string_ |