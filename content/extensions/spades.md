---
title: "SPAdes"
weight: 2900
---

# SPAdes

SPAdes – St. Petersburg genome assembler. Click [this link](http://bioinf.spbau.ru/en/spades) to open the SPAdes homepage. SPAdes is embedded as an [_external tool_](external-tools-plugin.md) into UGENE.

The SPAdes tool is available on macOS and Linux operating systems only.

Open _Tools ‣ NGS data analysis_.

![](/images/17467820/17631708.png)

Select the _Genome de novo assembly_ item to use _SPAdes_.

The _Assemble Genomes_ dialog will appear.

![](/images/17467820/17631707.png)

The following parameters are available:

_Output directory_ - SPAdes stores all output files in the output directory, which is set by the user.

_Library_ - to run SPAdes, choose one of the following libraries:

* Single-end
* Paired-end
* Paired-end (Interlaced)
* Paired-end (Unpaired files)
* Sanger
* PacBio

_Left reads_ - file(s) with left reads.

_Right reads_ - file(s) with right reads.

For each dataset in the paired-end libraries, you can change the type and orientation.

_Dataset type_ - dataset type.

_Running mode_ - running mode.

_k-mer sizes (-k)_ - k-mer sizes.

_Number of threads (-t)_ - number of threads.

_Memory limit GB (-m)_ - memory limit.