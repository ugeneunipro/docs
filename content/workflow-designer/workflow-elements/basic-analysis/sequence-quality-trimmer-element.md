---
title: "Sequence Quality Trimmer Element"
weight: 2100
---

# Sequence Quality Trimmer Element

This tool scans each input sequence from the end to find the first position where the quality is greater than or equal to the minimum quality threshold. It then trims the sequence to that position. If an entire sequence has quality less than the threshold or if the length of the output sequence is less than the minimum length threshold, the sequence is skipped.

**Element type:** SequenceQualityTrim

## Parameters

| Parameter | Description | Default Value | Parameter in Workflow File | Type |
|-----------|-------------|---------------|----------------------------|------|
| Trimming quality threshold | Quality threshold for trimming. | 30 | qual-id | _numeric_ |
| Min length | Too short reads are discarded by the filter. | 0 | len-id | _numeric_ |
| Trim both ends | Trim both ends of a read or not. Usually, you need to set **True** for **Sanger** sequencing and **False** for **NGS**. | True | both-ends | _boolean_ |

## Input/Output Ports

The element has 1 _input port_.

**Name in GUI:** _Input data_

**Name in Workflow File:** in-sequence

**Slots:**

| Slot In GUI | Slot in Workflow File | Type |
|-------------|-----------------------|------|
| Sequence    | sequence              | _sequence_ |

And 1 _output port_:

**Name in GUI:** _Output data_

**Name in Workflow File:** out-sequence

**Slots:**

| Slot In GUI | Slot in Workflow File | Type |
|-------------|-----------------------|------|
| Sequence    | sequence              | _sequence_ |