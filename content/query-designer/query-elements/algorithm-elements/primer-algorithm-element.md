---
title: "Primer Algorithm Element"
weight: 600
---

# Primer Algorithm Element

The _element_ searches primers against the input sequence.

Parameters in GUI
-----------------

| Parameter                  | Description                                                                                                              | Default value  |
|----------------------------|--------------------------------------------------------------------------------------------------------------------------|----------------|
| **Annotate As**            | Name of the result annotations.                                                                                          | top primers    |
| **Direction**              | See the description [_here_](http://ugene.unipro.ru/documentation/qd_manual/manipulating_schema/managing_strands.html#managing-strands). | Any            |
| **Excluded regions**       | The regions that should be avoided for primer selection.                                                                 | No default value. |
| **Max repeat mispriming**  | The maximum allowed weighted similarity with any sequence in the Mispriming Library.                                     | 12             |
| **Max template mispriming**| The maximum allowed similarity to ectopic sites in the sequence from which you are designing the primers.                | 12             |
| **Number to return**       | The maximum number of primer pairs to return.                                                                            | 5              |
| **Pair max repeat mispriming** | The maximum allowed sum of similarities of a primer pair (one similarity for each primer) with any single sequence in the Mispriming Library. | 24             |
| **Pair max template mispriming** | The maximum allowed summed similarity of both primers to ectopic sites in the sequence from which you are designing the primers. | 24             |
| **Product size ranges**    | List of product size ranges. The primer first tries to pick primers in the first range. If that is not possible, it goes to the next range and tries again. It continues in this way until it has either picked all necessary primers or until there are no more ranges. | 150-200, 100-300, 301-400, 401-500, 501-600, 601-700, 701-850, 851-1000 |
| **Max 3’ stability**       | The maximum stability for the last five 3’ bases of a left or right primer. Bigger numbers mean more stable 3’ ends.     | 9              |
| **Targets**                | If one or more Targets are specified, then a legal primer pair must flank at least one of them.                          | No default value. |

Parameters in Schema File
-------------------------

**Type:** primer

| Parameter                  | Parameter in the GUI                  | Type     |
|----------------------------|---------------------------------------|----------|
| **key**                    | **Annotate As**                       | _string_ |
| **excluded\_regions**      | **Excluded regions**                  | _string_ |
| **max\_mispriming**        | **Max repeat mispriming**             | _numeric_|
| **max\_template\_mispriming** | **Max template mispriming**         | _numeric_|
| **num\_return**            | **Number to return**                  | _numeric_|
| **pair\_max\_mispriming**  | **Pair max repeat mispriming**        | _numeric_|
| **pair\_max\_template\_mispriming** | **Pair max template mispriming** | _numeric_|
| **size\_ranges**           | **Product size ranges**               | _string_ |
| **stability**              | **Max 3’ stability**                  | _numeric_|
| **targets**                | **Targets**                           | _string_ |