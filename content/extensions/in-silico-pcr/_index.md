---
title: "In Silico PCR"
weight: 1100
---


# In Silico PCR

### In Silico PCR Overview

In silico PCR is used to calculate theoretical polymerase chain reaction (PCR) results using a given set of primers (probes) to amplify DNA sequences.

UGENE provides the In silico PCR feature only for nucleic sequences with Standard DNA and Extended DNA alphabets. To use it in UGENE open a DNA sequence and go to the _In silico PCR_ tab of the Options Panel:


![](/images/65930776/65930778.png)

There are the following parameters:

_Forward primer_ - forward primer. The primer length should be between 15 and 50 bases.

_Reverse primer_ - on the opposite strand from the forward primer. The primer length should be between 15 and 50 bases.

Note: you should take in account, that algorithm calculates no more than 50 forward and 50 reverse primers, which means, that you can take 50x50=2500 products maximum.

_Mismatches_ - mismatches limit.

_3' perfect match -_ specify the number of nucleotides at the 3' end that must not have mismatches.

_Maximum product size_ - the maximum size of the amplified sequence. _Use ambiguous bases -_ search for ambiguous bases (as \\"N\\") if checked.

_Extract annotations -_ specify the type of extracted annotations: _Inner, All intersected_ or _None_.

*   *   Value _Inner_ is selected by default. When this value is selected, the extracted PCR product contains annotations from the original sequence, located within the extracted region.
    *   Value _All intersected_ specifies that all annotations of the original sequence that intersect the extracted region must be extracted as well.
    *   Value _None_ specifies that annotations from the original sequence must not be extracted.

_Melting temperature_ - see [the corresponding page](https://doc.ugene.net/wiki/display/UM/Melting+tempeature) for details.

### Choosing primers

Type two primers for running In Silico PCR. If the primers pair is invalid for running the PCR process then the warning is shown. Also, primers for the running In silico PCR can be chosen from a [primer library](https://ugene.unipro.ru/wiki/display/UUOUM15/Primer+Library). Click the following button to choose a primer from the primers library:


![](/images/65930776/74809370.png)

 The following dialog will appear:


![](/images/65930776/65930779.png)

The table consists of the following columns: name, GC-content (%), Tm, Length (bp) and sequence. Select primer in the table and click the _Choose_ button.

Click the _Reverse-complement_ button for making a primer sequence reverse-complement:


![](/images/65930776/65930777.png)

Click _Show primers details_ for seeing [statistic details](https://ugene.unipro.ru/wiki/display/UUOUM15/Primers+Details) about primers.

When you run the process, the predicted PCR products appear in the products table.

### Melting temperature

Click the [Melting tempeature](https://doc.ugene.net/wiki/display/UM/Melting+tempeature) link for choosing temperature calculation algorithm: Rough or Primer 3.

More information about the temperature options see here:  [Melting tempeature](https://doc.ugene.net/wiki/display/UM/Melting+tempeature)

### Products table

There are three columns in the table:

*   region of product in the sequence
*   product length
*   preferred annealing temperature

 Click the product for navigating to its region in the sequence.

 Click the _Extract product(s)_ button for exporting a product(s) in a file or use double click for that.


![](/images/65930776/94078801.png)
