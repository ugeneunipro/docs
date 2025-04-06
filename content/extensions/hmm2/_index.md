---
title: "HMM2"
weight: 1
---


# HMM2

The _HMM2_ plugin is a toolkit based on Sean Eddy’s [HMMER2 package](http://hmmer.janelia.org/).

While working on this plugin we were guided by the following principles:

*   Make the HMMER2 tools accessible to a wider user audience by providing a graphical interface for all supported utilities for most of the platforms.
*   Be compatible with the original HMMER2 package.
*   Create a high-performance solution utilizing modern multi-core processors and SIMD instructions.

The current version of UGENE provides the user interface for three HMM2 tools: [_HMM build_](building-hmm2-model.md), _[HMM calibrate](calibrating-hmm2-model.md),_ and [_HMM search_](searching-sequence-using-hmm2-profile.md).

In the original program, the corresponding commands are: “hmmbuild”, “hmmcalibrate” and “hmmsearch”.

To access these tools select the _Tools ‣ HMMER tools_ submenu of the program main menu:


![](/images/54363779/54363780.png)

We highly recommend reading the [original HMMER2 documentation](http://hmmer.janelia.org/#documentation) to learn how to use utilities provided by the plugin.

SSE2 algorithm is implemented by Leonid Konyaev, Novosibirsk State University. Use of the SSE2 optimized version of the [_HMM search_](http://ugene.unipro.ru/documentation/manual/plugins/hmm2.html#hmm-search) algorithm with quad-core CPU gives >30x performance boost when compared with the original single-threaded algorithm (single sequence mode).

*   [Building HMM2 Model](building-hmm2-model.md)
*   [Calibrating HMM2 Model](calibrating-hmm2-model.md)
*   [Searching Sequence Using HMM2 Profile](searching-sequence-using-hmm2-profile.md)


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
