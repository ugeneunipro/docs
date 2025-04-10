---
title: "De novo Assembly of Illumina PE and Nanopore Reads"
weight: 800
---

# De novo Assembly of Illumina PE and Nanopore Reads

The workflow sample described below takes FASTQ files with paired-end Illumina reads and FASTQ file(s) with Oxford Nanopore reads and assembles these data de novo using SPAdes.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, refer to the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

### Workflow Sample Location

The workflow sample "De novo Assembly of Illumina PE and Nanopore Reads" can be found in the "NGS" section of the Workflow Designer samples.

### Workflow Image

The opened workflow looks as follows:

![](/images/65930362/65930363.jpg)

### Workflow Wizard

The wizard has four pages.

#### 1. Input Data: Illumina Reads

On this page, you must set files with Illumina reads.

![](/images/65930362/65930364.jpg)

#### 2. Input Data: Nanopore Reads

You must set the Nanopore reads on this page.

![](/images/65930362/65930365.jpg)

#### 3. SPAdes Settings

You can change the default SPAdes parameters here.

![](/images/65930362/65930366.jpg)

The following parameters are available:

| Parameter            | Description                                                                                                                                                                     |
|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Dataset type**     | Select the input dataset type:<br>- **Standard isolate** *(default)*<br>- **Multiple displacement amplification** (`--sc`)                                                     |
| **Running mode**     | By default, SPAdes performs both **read error correction** and **assembly**.<br>You can select one of the modes:<br>- `--only-error-correction` — only error correction<br>- `--only-assembler` — only assembly |
| **Error correction** | - **BayesHammer** is used for Illumina reads<br>- **IonHammer** is used for IonTorrent reads<br>⚠️ Do not use error correction if input reads have no quality data (e.g., FASTA input files are provided)          |
| **K-mers**           | Set one or more k-mer sizes (`-k`) to be used during assembly. If not specified, SPAdes will choose values automatically based on read length.                                                |

#### 4. Output Files Page

On this page, you can select an output directory:

![](/images/65930362/65930367.jpg)
