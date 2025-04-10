---
title: "Read Annotations Element"
weight: 200
---

# Read Annotations Element

Input one or several files with annotations: a file may also contain a sequence (e.g., GenBank format) or contain annotations only (e.g., GTF format).

The element outputs messages with the annotations data.

See the list of all available formats [here](https://ugene.net/wiki/display/UUOUM27/Appendix+A.+Supported+File+Formats).

**Element type:** read-annotations

Parameters
----------

| Parameter        | Description                                                                                                                                                           | Default value   | Parameter in Workflow File | Type           |
|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------|----------------------------|----------------|
| **Input file(s)** | Input files.                                                                                                                                                          | Dataset 1       | **url-in**                 | _string_       |
| **Mode**         | If the file contains more than one annotation table, Split mode sends them "as is" to the output, while Merge appends all the annotation tables and outputs the sole merged annotation table. In Merge, files is the same as Merge but it operates with all annotation tables from all files of one dataset. | Merge           | **mode**                   | _numeric_      |

Input/Output Ports
------------------

The element has 1 _output port_:

| Name in GUI          | Name in Workflow File | Type                  |
|----------------------|-----------------------|-----------------------|
| **Annotations**      | **out-annotations**   |                       |
| **Set of annotations** | **annotations**        | _annotation-table-list_|
| **Dataset name**     | **dataset**           | _string_              |
| **Source URL**       | **out-url**           | _string_              |