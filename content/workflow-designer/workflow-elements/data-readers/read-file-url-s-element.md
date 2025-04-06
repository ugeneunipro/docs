---
title: "Read File URL(s) Element"
weight: 1
---


# Read File URL(s) Element

Input one or several files in any format. The element outputs the file(s) URL(s).

**Element type:** get-file-list

Parameters in GUI
-----------------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Input directory**

Input directory.



**in-path**

_string_



Specify whether to output absolute or relative paths of the files.

True

**absolute**

_boolean_

**Recursive reading**

Get files from all nested directories or just from the current one.

False

**recursive**

_boolean_

**Include name filter**

Filter files by the specified value. It can be, for example, a file name or a regular expression of the file name.



**include-name-filter**

_string_

**Exclude name filter**

Exclude files using the specified filter value. The value can be, for example, a file name or a regular expression of the file name.



**exclude-name-filter**

_string_



Input/Output Ports
------------------

The element has 1 _output port_:

**Name in GUI:** _out-url_

**Name in Workflow File:** out-url

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**Source URL**

**out-url**

_string_
