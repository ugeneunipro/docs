---
title: "Read Plain Text Element"
weight: 700
---

# Read Plain Text Element

Input one or several text files. The element outputs text message(s) read from the file(s).

See the list of all available formats [here](https://ugene.net/wiki/display/UUOUM27/Appendix+A.+Supported+File+Formats).

**Element type:** read-text

Parameters
----------

| Parameter          | Description                             | Default value | Parameter in Workflow File | Type    |
|--------------------|-----------------------------------------|---------------|-----------------------------|---------|
| **Input files**    | Semicolon-separated list of paths to the input files. |               | **url-in**                  | _string_ |
| **Read by lines**  | Specifies to read the input file line by line.         | false         | **read-by-lines**           | _boolean_ |

Input/Output Ports

The element has 1 _output port_:

| Slot In GUI  | Slot in Workflow File |
|--------------|-----------------------|
| **Plain text** | **text**             |
| **Source URL** | **url**              |

- **Name in GUI:** _Plain text_
- **Name in Workflow File:** out-text