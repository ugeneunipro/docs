---
title: "Map to Reference Element"
weight: 1200
---

# Map to Reference Element

Align input sequences (e.g., Sanger reads) to the reference sequence.

**Element type:** align-to-reference

Parameters
----------

| Parameter         | Description                              | Default value | Parameter in Workflow File |
|-------------------|------------------------------------------|---------------|----------------------------|
| **Reference URL** | A URL to the file with a reference sequence. |               | **reference**              |
| **Type**          |                                           |               | _string_                   |

Input/Output Ports
------------------

The element has 1 _input port_:

**Name in GUI:** Input sequence

**Name in Workflow File:** in-sequence

**Slots:**

| Slot In GUI | Slot in **Workflow** File | Type      |
|-------------|---------------------------|-----------|
| **Sequence** | sequence                  | _sequence_ |

And 1 _output port_:

**Name in GUI:** Aligned data

**Name in Workflow File:** out

**Slots:**

| Slot In GUI           | Slot in **Workflow** File | Type         |
|-----------------------|---------------------------|--------------|
| **Set of annotations** | annotations               | _ann_table_  |
| **MSA**               | msa                       | _malignment_ |
| **Sequence**          | sequence                  | _sequence_   |