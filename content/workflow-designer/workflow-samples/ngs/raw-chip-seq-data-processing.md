---
title: "Raw ChIP-Seq Data Processing"
weight: 1800
---

# Raw ChIP-Seq Data Processing

The component for ChIP-seq data analysis is not installed by default. To use this sample, add the component via the UGENE Online Installer or, if you used an offline installer, manually configure the package. See the "[Configure ChIP-seq Analysis Data](/wiki/pages/createpage.action?spaceKey=UM&title=Configure+ChIP-Seq+Analysis+Data&linkCreation=true&fromPageId=65930463)" chapter of the manual.

Use this workflow sample to process raw ChIP-seq next-generation sequencing (NGS) data from the Illumina platform. The processing includes:

* _Filtration:_
  * Filtering of the NGS short reads by the CASAVA 1.8 header;
  * Trimming of the short reads by quality;
* _Mapping:_
  * Mapping of the short reads to the specified reference sequence (the BWA-MEM tool is used in the sample);
* _Post-filtration:_
  * Filtering of the aligned short reads by SAMtools to remove reads with low mapping quality, unpaired/unaligned reads;
  * Removing of duplicated short reads.

The result of the data processing is provided in the BED format. Intermediate data files from the filtration and mapping steps are also available in the output.

## How to Use This Sample

If you haven't used the workflow samples in UGENE before, look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Raw ChIP-Seq Processing" can be found in the "NGS" section of the Workflow Designer samples.

##### Workflow Image

There are two versions of the workflow available. The workflow for single-end reads looks as follows:

![](/images/65930463/65930464.png)

The workflow for paired-end short reads appears as follows:

![](/images/65930463/65930465.png)

##### Workflow Wizard

The workflows have similar wizards. The wizard for paired-end reads has 5 pages.

1. **Input Data**: On this page, you must input FASTQ file(s).

   ![](/images/65930463/65930466.png)

2. **Pre-processing**: On this page, you can modify filtration parameters.

   ![](/images/65930463/65930467.png)

   The following parameters are available for reads and reads pairs filtration:

   | Parameter         | Description |
   |-------------------|-------------|
   | Base quality      | Quality threshold for trimming. |
   | Reads length      | Too short reads are discarded by the filter. |
   | Trim both ends    | Trim both ends of a read or not. Usually, set True for Sanger sequencing and False for NGS. |
   | 3' adapters       | A FASTA file with one or multiple sequences of adapter that were ligated to the 3' end. The adapter itself and anything that follows is trimmed. If the adapter sequence ends with the '$' character, the adapter is anchored to the end of the read and only found if it is a suffix of the read. |
   | 5' adapters       | A FASTA file with one or multiple sequences of adapters that were ligated to the 5' end. If the adapter sequence starts with the character '^', the adapter is 'anchored'. An anchored adapter must appear in its entirety at the 5' end of the read (it is a prefix of the read). A non-anchored adapter may appear partially at the 5' end or may occur within the read. If it is found within a read, the sequence preceding the adapter is also trimmed. In all cases, the adapter itself is trimmed. |
   | 5' and 3' adapters| A FASTA file with one or multiple sequences of adapter that were ligated to the 5' end or 3' end. |

3. **Mapping**: On this page, you must input a reference and optionally modify advanced parameters.

   ![](/images/65930463/65930468.png)

   The following parameters are available:

   | Parameter             | Description |
   |-----------------------|-------------|
   | Reference genome      | Path to indexed reference genome. |
   | Number of threads     | Number of threads (-t). |
   | Min seed length       | Min seed length (-k). |
   | Band width            | Band width for banded alignment (-w). |
   | Dropoff               | Off-diagonal X-dropoff (-d). |
   | Internal seed length  | Look for internal seeds inside a seed longer than {-k} (-r). |
   | Skip seed threshold   | Skip seeds with more than INT occurrences (-c). |
   | Drop chain threshold  | Drop chains shorter than FLOAT fraction of the longest overlapping chain (-D). |
   | Rounds of mate rescues| Perform at most INT rounds of mate rescues for each read (-m). |
   | Skip mate rescue      | Skip mate rescue (-S). |
   | Skip pairing          | Skip pairing; mate rescue performed unless -S also in use (-P). |
   | Mismatch penalty      | Penalty for a mismatch (-B). |
   | Gap open penalty      | Gap open penalty (-O). |
   | Gap extension penalty | Gap extension penalty; a gap of size k costs {-O} (-E). |
   | Penalty for clipping  | Penalty for clipping (-L). |
   | Penalty unpaired      | Penalty for an unpaired read pair (-U). |
   | Score threshold       | Minimum score to output (-T). |

4. **Post-processing**: On this page, you can modify post-processing parameters.

   ![](/images/65930463/65930469.png)

   The following parameters are available:

   | Parameter    | Description |
   |--------------|-------------|
   | MAPQ threshold| Minimum MAPQ quality score. |
   | Skip flag     | Skip alignment with the selected items. Select the items in the combobox to configure the bit flag. Do not select the items to avoid filtration by this parameter. |
   | Region        | Regions to filter. For BAM output only. Use 'chr2' to output the whole chr2. '[chr2:1000]' to output regions of chr2 starting from 1000. '[chr2:1000-2000]' to output regions of chr2 between 1000 and 2000 including the endpoint. To input multiple regions, use the space separator (e.g. chr1 chr2 [chr3:1000-2000]). |
   | For single-end reads | Remove duplicates for single-end reads. |

5. **Output Data**: On this page, you must input output parameters.

   ![](/images/65930463/65930470.png)