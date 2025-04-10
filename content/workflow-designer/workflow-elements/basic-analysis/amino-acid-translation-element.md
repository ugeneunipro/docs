---
title: "Amino Acid Translation Element"
weight: 100
---

# Amino Acid Translation Element

Translates a sequence into its amino acid translation or translations.

**Element type:** sequence-translation

## Parameters

| Parameter                      | Description                                                                                                                                           | Default value             | Parameter in Workflow File | Type      |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|----------------------------|-----------|
| **Translate from**             | Specifies the position that should be used to translate the sequence from: first, second, third, or all (which would generate three output amino acid sequences). | all                       | **pos-2-translate**        | _string_  |
|                                | Available values are:<br>• all<br>• first<br>• second<br>• third                                                                                      |                           |                            |           |
| **Auto-selected genetic code** | Specifies that the genetic code should be selected automatically.                                                                                     | True                      | **auto-translation**       | _boolean_ |
| **Genetic code**               | The genetic code that should be used to translate the input nucleotide sequence.                                                                       | The Standard Genetic Code | **genetic-code**           | _string_  |

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input Data_  
**Name in Workflow File:** in-sequence  
**Slots:**

| Slot in GUI  | Slot in Workflow File | Type       |
|--------------|-----------------------|------------|
| **Sequence** | **sequence**          | _sequence_ |

And 1 _output port_:

**Name in GUI:** _Amino sequence_  
**Name in Workflow File:** out-sequence  
**Slots:**

| Slot in GUI    | Slot in Workflow File | Type       |
|----------------|-----------------------|------------|
| **Sequence**   | **sequence**          | _sequence_ |
| **Plain text** | **text**              | _string_   |