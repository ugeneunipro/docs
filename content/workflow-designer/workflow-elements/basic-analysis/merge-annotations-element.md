---
title: "Merge Annotations Element"
weight: 1800
---


# Merge Annotations Element

Writes all supplied sequences to file(s) in FASTQ format.

**Element type:** write-fastq

Parameters
----------

| Parameter          | Description                                                                                                                                                                     | Default value | Parameter in Workflow File | Type     |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|----------|
| **Output file**    | Location of the output data file. If this attribute is set, then the “Location” slot is not taken into account.                                                                  |               | url-out                    | _string_ |
| **Existing file**  | If a target file already exists, you can specify how it should be handled: either overwritten, renamed, or appended (if supported by the file format). Available values are:      | Rename        | write-mode                 | _numeric_|
|                    | 0 - for overwrite<br> 1 - for append<br> 2 - for rename                                                                                                                         |               |                            |          |
| **Accumulate objects** | Accumulates all incoming data in one file or creates separate files for each input. In the latter case, an incremental numerical suffix is added to a file name.          | True          | accumulate                 | _boolean_|

Input/Output Ports
------------------

The element has 1 _input port_:

- **Name in GUI:** _Sequence_
- **Name in Workflow File:** in-sequence

| Slot In GUI | Slot in Workflow File | Type       |
|-------------|-----------------------|------------|
| **Sequence**| sequence              | _sequence_ |
| **Location**| url                   | _string_   |