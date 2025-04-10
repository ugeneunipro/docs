---
title: "Split Assembly into Sequences Element"
weight: 500
---


# Split Assembly into Sequences Element

Splits assembly into sequences (reads).

**Element type:** reverse-complement

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** in-assembly

**Name in Workflow File:** in-assembly

**Slots:**

| Slot In GUI     | Slot in Workflow File | Type      |
|-----------------|-----------------------|-----------|
| Assembly data   | assembly              | _assembly_|

And 1 _output port_:

**Name in GUI:** out-sequence

**Name in Workflow File:** out-sequence

**Slots:**

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| Sequence    | seq                   | _string_ |