---
title: "Map NGS Reads with UGENE Genome Aligner"
weight: 300
---


# Map NGS Reads with UGENE Genome Aligner

When you select the _Tools ‣ NGS Data analysis‣ Map reads to reference_ item in the main menu, the _Map NGS Reads to Reference_ dialog appears. Set the _Mapping tool_ parameter to _UGENE Genome Aligner_. The dialog looks as follows:


![](/images/65930891/65930892.png)

The following parameters are available:

_Reference sequence_ — DNA sequence to align short reads to. This parameter is required.

_Result file name_ — file in UGENE database format or SAM format (if the box _SAM output_ check), to write the result of the alignment into. This parameter is required.

_Prebuilt index_ — check this box to use an index file instead of a reference sequence. Also you can [_build it manually_](http://ugene.unipro.ru/documentation/manual/plugins/bwa/build_index.html#bwa-build-index).

_SAM output_ — checking this box allows one to save output files in the SAM format. The default format of output files is the UGENE database format (ugenedb).

_Short reads_ — each added short read is a small DNA sequence file. At least one read should be added.

The _Map NGS Reads with UGENE Genome Aligner_ has no limitation on short reads length.

_Common parameters_:

_Mismatches allowed_ — check this box to allow mismatches between the reference sequence and a short read. Select one of the following:

*   *   _Mismatches number_ to set the number of mismatched nucleotides allowed. This parameter can take values: 1, 2 and 3.
    *   _Percentage of mismatches_ to set the number of mismatches in percents. Note, that in this case the absolute number of mismatches can vary for different reads. This parameter can take values: 1 - 10 %.

_Align options_:

*   *   _Use GPU-optimization_ — use an openCL-enabled GPU during the alignment (the corresponding hardware should be available on your computer). This option was available until v44.
    *   _Align reverse complement reads_ — use both: a read and its reverse complement during the alignment.
    *   _Use “best”-mode during the alignment_ — report only about best alignments (in terms of mismatches).
    *   _Omit reads with qualities lower than_ — omit all reads with qualities lower than the specified value. Reads that have no qualities are not omited.

_Advanced parameters_:

_Maximum memory for short reads_ — maximum memory usage for short reads. This parameter allows one to decrease the load on the computer on one side and to increase the computer speed of the task on the other side.

*   *   _Total memory usage_ — shows the total memory usage.
    *   _System memory size_ — shows the total system memory size.

_Index parameters_:

_Reference fragmentation_ — this parameter influences the number of parts the reference will be divided. It is better to make it bigger, but it influences the amount of memory used during the alignment.

*   *   _Index memory usage size_ — shows the index memory usage.
    *   _Directory for index files_ — temporary directory for saving index files.

You can choose a temporary directory for saving index files for the reference that will be built during the alignment. If you need to run this algorithm one more time with the same reference and with the same reference fragmentation parameter, you can use this prebuilt index that will be located in the temporary directory.
