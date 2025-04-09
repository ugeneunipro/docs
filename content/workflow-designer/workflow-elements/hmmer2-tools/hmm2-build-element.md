---
title: "HMM2 Build Element"
weight: 100
---


# HMM2 Build Element

Builds a HMM profile from a multiple sequence alignment. The HMM profile is a statistical model which captures position-specific information about how conserved each column of the alignment is, and which residues are likely.

**Element type:** hmm2-build

Parameters
----------

Parameter

Description

Default value

Parameter in Workflow File

Type

**Profile name**

Descriptive name of the HMM profile.



**profile-name**

_string_

**HMM strategy**

Specifies the kind of alignments you want to allow.

hmmls

**strategy**

_numeric_

Available values are:

*   0 - for hmms
*   1 - for hmmls
*   2 - for hmmfs
*   3 - for hmmsw

**Calibrate profile**

Enables/disables optional profile calibration. An empirical HMM calibration costs time but it only has to be done once per model, and can greatly increase the sensitivity of a database search.

True

**calibrate**

_boolean_

**Parallel calibration**

Number of parallel threads that the calibration will run in.

1

**calibration-threads**

_numeric_

**Standard deviation**

Standard deviation of the synthetic sequence length. A positive number. Note that the Gaussian is left-truncated so that no sequences have lengths.

200.0

**deviation**

_numeric_

**Fixed length of samples**

Fixes the length of the random sequences to, where is a positive (and reasonably sized) integer. The default is instead to generate sequences with a variety of different lengths, controlled by a Gaussian (normal) distribution.

0

**fix-samples-length**

_numeric_

**Mean length of samples**

Mean length of the synthetic sequences, positive real number.

325

**mean-samples-length**

_numeric_

**Number of samples**

Number of synthetic sequences. If is less than about 1000, the fit to the EVD may fail Higher numbers of will give better determined EVD parameters. The default is 5000; it was empirically chosen as a tradeoff between accuracy and computation time.

5000

**samples-num**

_numeric_

**Random seed**

The random seed, where is a positive integer. The default is to use time() to generate a different seed for each run, which means that two different runs of hmmcalibrate on the same HMM will give slightly different results. You can use this option to generate reproducible results for different hmmcalibrate runs on the same HMM.

0

**seed**

_numeric_

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** _Input MSA_

**Name in Workflow File:** in-msa

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**MSA**

**msa**

_msa_

And 1 _output port_:

**Name in GUI:** _HMM profile_

**Name in Workflow File:** out-hmm2

**Slots:**

Slot In GUI

Slot in Workflow File

Type

**HMM profile**

**hmm2-profile**

_hmm2-profile_
