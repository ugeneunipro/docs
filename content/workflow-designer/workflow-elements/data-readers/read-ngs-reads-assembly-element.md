---
title: "Read NGS Reads Assembly Element"
weight: 600
---

# Read NGS Reads Assembly Element

Input one or several files with assembled NGS reads in SAM, BAM, or UGENEDB format.

The element outputs message(s) with the assembled reads data.

See the list of all available formats [here](https://ugene.net/wiki/display/UUOUM27/Appendix+A.+Supported+File+Formats).

**Element type:** read-assembly

Parameters
----------

| Parameter         | Description | Default value | Parameter in Workflow File | Type   |
|-------------------|-------------|---------------|----------------------------|--------|
| **Input file(s)** | Input files | Dataset 1     | **url-in**                 | _string_ |

Input/Output Ports
------------------

The element has 1 _output port_:

| Name in GUI      | Name in Workflow File | Type       |
|------------------|-----------------------|------------|
| **Assembly**     | out-assembly          |            |
| **Slots:**       |                       |            |
| Slot In GUI      | Slot in Workflow File | Type       |
| **Assembly data**| **assembly**          | _assembly_ |
| **Dataset name** | **dataset**           | _string_   |
| **Source URL**   | **out-url**           | _string_   |