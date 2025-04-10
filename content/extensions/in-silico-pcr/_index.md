---
title: "In Silico PCR"
weight: 1100
---

# In Silico PCR

### In Silico PCR Overview

In silico PCR is used to calculate theoretical polymerase chain reaction (PCR) results using a given set of primers (probes) to amplify DNA sequences.

UGENE provides the In silico PCR feature only for nucleic sequences with Standard DNA and Extended DNA alphabets. To use it in UGENE, open a DNA sequence and go to the _In silico PCR_ tab of the Options Panel:

![](/images/65930776/65930778.png)

The parameters are as follows:

- _Forward primer_: The forward primer. The primer length should be between 15 and 50 bases.
  
- _Reverse primer_: The reverse primer on the opposite strand from the forward primer. The primer length should be between 15 and 50 bases.
  
Note: You should take into account that the algorithm calculates no more than 50 forward and 50 reverse primers, which means that you can have a maximum of 2500 products.

- _Mismatches_: The mismatches limit.
  
- _3' perfect match_: Specify the number of nucleotides at the 3' end that must not have mismatches.

- _Maximum product size_: The maximum size of the amplified sequence.

- _Use ambiguous bases_: Search for ambiguous bases (e.g., "N") if checked.

- _Extract annotations_: Specify the type of extracted annotations: _Inner, All intersected_, or _None_.
  - Value _Inner_ is selected by default. When this value is selected, the extracted PCR product contains annotations from the original sequence, located within the extracted region.
  - Value _All intersected_ specifies that all annotations of the original sequence that intersect the extracted region must be extracted as well.
  - Value _None_ specifies that annotations from the original sequence must not be extracted.

- _Melting temperature_: See [the corresponding page](https://doc.ugene.net/wiki/display/UM/Melting+tempeature) for details.

### Choosing Primers

Type two primers for running In Silico PCR. If the primer pair is invalid for running the PCR process, a warning is shown. Primers for the running In silico PCR can also be chosen from a [primer library](https://ugene.unipro.ru/wiki/display/UUOUM15/Primer+Library). Click the following button to choose a primer from the primers library:

![](/images/65930776/74809370.png)

The following dialog will appear:

![](/images/65930776/65930779.png)

The table consists of the following columns: name, GC-content (%), Tm, length (bp), and sequence. Select a primer in the table and click the _Choose_ button.

Click the _Reverse-complement_ button to make a primer sequence reverse-complementary:

![](/images/65930776/65930777.png)

Click _Show primers details_ to see [statistical details](https://ugene.unipro.ru/wiki/display/UUOUM15/Primers+Details) about primers.

When you run the process, the predicted PCR products appear in the products table.

### Melting Temperature

Click the [Melting temperature](https://doc.ugene.net/wiki/display/UM/Melting+tempeature) link for choosing a temperature calculation algorithm: Rough or Primer 3.

For more information about temperature options, see here: [Melting temperature](https://doc.ugene.net/wiki/display/UM/Melting+tempeature).

### Products Table

There are three columns in the table:

- Region of the product in the sequence
- Product length
- Preferred annealing temperature

Click the product to navigate to its region in the sequence.

Click the _Extract product(s)_ button to export a product(s) to a file or double click to do that.

![](/images/65930776/94078801.png)