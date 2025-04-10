---
title: "Convert Text to Sequence Element"
weight: 200
---

# Convert Text to Sequence Element

Converts the input text into a sequence.

**Element type:** convert-text-to-sequence

## Parameters

| Parameter                    | Description                                                                                                                                                                                 | Default value | Parameter in Workflow File | Type      |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Sequence name** (required) | Result sequence name.                                                                                                                                                                       | _Sequence_    | **sequence-name**          | _string_  |
| **Sequence alphabet**        | Alphabet of the sequence. Choose _Auto_ to auto-detect, or select:<br>• _All symbols_<br>• _Extended DNA_<br>• _Extended RNA_<br>• _Standard DNA_<br>• _Standard RNA_<br>• _Standard amino_ | _Auto_        | **alphabet**               | _string_  |
| **Skip unknown symbols**     | If _True_, ignores symbols not in the selected alphabet.                                                                                                                                    | _True_        | **skip-unknown**           | _boolean_ |
| **Replace unknown with**     | Replaces unknown symbols with a specified character.                                                                                                                                        | _N_           | **replace-unknown-with**   | _string_  |

## Input/Output Ports

| Port Name (GUI)     | Workflow File Name | Slots                                  |
|---------------------|--------------------|----------------------------------------|
| **Input text**      | `in-text`          | **Plain text** → `text` (_string_)     |
| **Output sequence** | `out-sequence`     | **Sequence** → `sequence` (_sequence_) |