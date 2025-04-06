---
title: "Base Content Algorithm Element"
weight: 1
---


# Base Content Algorithm Element

Searches regions in a sequence that contain a specified percentage of a certain base.

Parameters in GUI
-----------------

Parameter

Description

Default value

**Annotate As**

Name of the result annotations.

misc\_feature

**Base**

Specifies the base, i.e. A, C, G or T.

You must specify a value!

**Percentage**

Percentage of the base in a region. The value must be >= 50%.

90%

**Min Length**

Minimum length of a region. The value must be >= 5.

5 bp

**Max Length**

Maximum length of a region.

5 bp

**Direction**

See the description [_here_](http://ugene.unipro.ru/documentation/qd_manual/manipulating_schema/managing_strands.html#managing-strands).

Any

Parameters in Schema File
-------------------------

**Type:** base-content

Parameter

Parameter in the GUI

Type

**key**

**Annotate As**

_string_

**base**

**Base**

_string_

**percent**

**Percentage**

_numeric_

**min-len**

**Min Length**

_numeric_

**max-len**

**Max Length**

_numeric_
