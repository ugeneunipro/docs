---
title: "HMM3 Algorithm Element"
weight: 400
---

# HMM3 Algorithm Element

The algorithm searches a sequence for significantly similar sequence matches with one or more profile HMMs and saves the results as annotations.

The search is performed using the HMMER3 **hmmsearch** tool integrated into UGENE.

## Parameters in GUI

**General parameters:**

| Parameter    | Description                       | Default value |
|--------------|-----------------------------------|---------------|
| **Annotate As** | Name of the result annotations.    | hmm_signal    |
| **Profile HMM** | Semicolon-separated list of input HMM files. You must specify a value! |               |
| **Min Length**  | Minimum length of a result region. | 30            |
| **Max Length**  | Maximum length of a result region. | 5000          |

**Parameters controlling reporting threshold:**

Reporting thresholds control which hits are reported.

| Parameter               | Description                                                                                                     | Default value |
|-------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|
| **Use E-value**         | Filter by E-value if true. Otherwise, filter by score.                                                          | True          |
| **Filter by High E-value** | Reports domains ≤ this E-value threshold in output (**hmmsearch**–domE option).                             | 1e+1          |
| **Filter by Low Score** | Reports domains ≥ this score cutoff in output (**hmmsearch**–domT option).                                      | 0.01          |

**Parameters controlling the acceleration pipeline:**

HMMER3 searches are accelerated in a three-step filter pipeline: the MSV filter, the Viterbi filter, and the Forward filter. The first filter is the fastest and most approximate; the last is the full Forward scoring algorithm. There is also a bias filter step between MSV and Viterbi.

| Parameter                  | Description                                                                                                             | Default value |
|----------------------------|-------------------------------------------------------------------------------------------------------------------------|---------------|
| **Max**                   | Turns off all acceleration heuristic filters. This increases sensitivity somewhat, at a large cost in speed.           | False         |
| **MSV Filter Threshold**  | P-value threshold for the MSV filter step.                                                                               | 0.02          |
| **Viterbi Filter Threshold** | P-value threshold for the Viterbi filter step.                                                                        | 0.001         |
| **Forward Filter Threshold** | P-value threshold for the Forward filter step.                                                                      | 1e-5          |
| **No Bias Filter**         | Turns off composition bias filter. This increases sensitivity somewhat, but can come at a high cost in speed.          | False         |

**Other parameters:**

| Parameter                | Description                                                                                                           | Default value |
|--------------------------|-----------------------------------------------------------------------------------------------------------------------|---------------|
| **No Null2**             | Turns off the null2 score corrections for biased composition.                                                         | False         |
| **Number of Sequences**  | Specifies the number of significant sequences. It is used for domain E-value calculations (**hmmsearch**–domZ option). | 1 (i.e., one input sequence) |
| **Seed**                 | Random number seed. The default is to use a fixed seed (42), so that results are exactly reproducible. Any other positive integer will give different (but also reproducible) results. A choice of 0 uses a randomly chosen seed. | 42            |

## Parameters in Schema File

| Type: hmm3                  |
|-----------------------------|
| **Parameter**                | **Parameter in the GUI** | **Type**         |
|------------------------------|--------------------------|------------------|
| **key**                      | **Annotate As**          | _string_         |
| **min-len**                  | **Min Length**           | _string_         |
| **max-len**                  | **Max Length**           | _string_         |
| **hmm-profile**              | **Profile HMM**          | _string_         |
| **use-e-val**                | **Use E-value**          | _boolean_        |
| **e-val**                    | **Filter by High E-value**       | _numeric_        |
| **score**                    | **Filter by Low Score**  | _numeric_        |
| **do-max**                   | **Max**                  | _boolean_        |
| **msv-filter-threshold**     | **MSV Filter Threshold** | _numeric_        |
| **viterbi-filter-threshold** | **Viterbi Filter Threshold**  | _numeric_        |
| **forward-filter-threshold** | **Forward Filter Threshold** | _numeric_        |
| **no-bias-filter**           | **No Bias Filter**       | _boolean_        |
| **no-score-corrections**     | **No Null2**             | _boolean_        |
| **seqs-num**                 | **Number of Sequences**  | _numeric_        |
| **random-generator-seed**    | **Seed**                 | _numeric_        |
