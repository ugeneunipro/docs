---
title: "De novo Assemble Illumina PE Reads"
weight: 700
---

# De novo Assemble Illumina PE Reads

The workflow sample, described below, takes FASTQ files with paired-end Illumina reads as input and processes them as
follows:

* Improve reads quality with Trimmomatic
* Provide FastQC quality reports
* De novo assemble reads with SPAdes

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at
the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

---

### Workflow Sample Location

The workflow sample **"De novo Assemble Illumina PE Reads"** can be found in the **"NGS"** section of the Workflow
Designer samples.

---

### Workflow Image

The opened workflow looks as follows:

![](/images/65930355/65930356.jpg)

---

### Workflow Wizard

The wizard has 4 pages.

---

#### 1. Input data: Illumina paired-end reads

On this page, files with Illumina paired-end reads must be set.

![](/images/65930355/65930357.jpg)

---

#### 2. Trimmomatic settings

The Trimmomatic parameters can be changed here:

![](/images/65930355/65930358.jpg)

To configure trimming steps use the following button:

![](/images/65930355/65930359.jpg)

The following dialog will appear:

![](/images/65930355/65930360.jpg)

Click the _**Add new step**_ button and select a step. The following options are available:

- **ILLUMINACLIP**
- **SLIDINGWINDOW**
- **LEADING**
- **TRAILING**
- **CROP**
- **HEADCROP**
- **MINLEN**
- **AVGQUAL**
- **TOPHRED33**
- **TOPHRED64**

Each step has its own parameters (see original document for detailed explanations).

To remove a step use the _**Remove selected step**_ button. The pink highlighting means the required parameter has not
been set.

---

#### 3. SPAdes settings

Default SPAdes parameters can be changed here.

##### Parameters Table

| **Parameter**        | **Description**                                                                                                                                                                                |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Dataset type**     | Select the input dataset type:<br>- Standard isolate (**default**)<br>- Multiple displacement amplification (`--sc`)                                                                           |
| **Running mode**     | By default, SPAdes performs both **read error correction** and **assembly**.<br>You can select:<br>- `--only-assembler` (assembly only)<br>- `--only-error-correction` (error correction only) |
| **Error correction** | SPAdes uses:<br>- **BayesHammer** for Illumina<br>- **IonHammer** for IonTorrent<br><br>⚠️ Do not use error correction with reads lacking quality info (e.g., FASTA)                           |
| **K-mers**           | Specify `-k` k-mer sizes. If not set, SPAdes selects them automatically based on read length                                                                                                   |

---

#### 4. Output Files Page

On this page, you can select an output directory.
