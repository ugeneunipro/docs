---
title: "Reverse Complement Element"
weight: 400
---

# Reverse Complement Element

This component converts an input sequence into its reverse, complement, or reverse-complement counterpart.

**Element type:** reverse-complement

Parameters
----------

| Parameter        | Description                                                             | Default value          | Parameter in Workflow File | Type    |
|------------------|-------------------------------------------------------------------------|------------------------|----------------------------|---------|
| **Operation type** | Selects whether to produce the reverse, complement, or reverse-complement sequence. | Reverse Complement     | **op-type**                | _string_ |

Available values are:

- reverse-complement
- complement
- reverse

Input/Output Ports
------------------

The element has 1 _input port_:

- **Name in GUI:** _Input sequence_
- **Name in Workflow File:** in-sequence

| Slot in GUI | Slot in Workflow File | Type      |
|-------------|-----------------------|-----------|
| **Sequence**  | **sequence**            | _sequence_ |

And 1 _output port_:

- **Name in GUI:** _Output sequence_
- **Name in Workflow File:** out-sequence

| Slot in GUI | Slot in Workflow File | Type      |
|-------------|-----------------------|-----------|
| **Sequence**  | **sequence**            | _sequence_ |