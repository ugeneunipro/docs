---
title: "Building PWM"
weight: 2100
---

# Building PWM

**Task Name:** pwm-build

This task builds a position weight matrix (PWM) from a multiple sequence alignment (MSA) file.

**Parameters:**

- **_in_** — a semicolon-separated list of input MSA files. \[String, Required\]

- **_out_** — the output file. \[String, Required\]

- **_type_** — type of the matrix. \[Boolean, Optional, Default: false\]

  The following values are available:

  - **true** (dinucleic type)
  - **false** (mononucleic type)

  Dinucleic matrices are more detailed, while mononucleic ones are more useful for small input data sets.

- **_algo_** — the algorithm used to build the matrix. \[String, Optional, Default: “Berg and von Hippel”\]

  The available options are:

  - Berg and von Hippel
  - Log-odds
  - Match
  - NLG

**Example:**

```bash
ugene pwm-build --in=COI.aln --out=result.pwm