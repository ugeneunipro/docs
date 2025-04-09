---
title: "HMM3"
weight: 1700
---


# HMM3

The _HMM3_ plugin is a toolkit based on Sean Eddy’s [HMMER3 package](http://hmmer.janelia.org/).

While working on this plugin we were guided by the following principles:

*   Make the HMMER3 tools accessible to a wider user audience by providing a graphical interface for all supported utilities for most of the platforms.
*   Be compatible with the original HMMER3 package.
*   Create a high-performance solution utilizing modern multi-core processors.

The current version of UGENE provides a user interface for three HMM3 tools: [_HMM3 build_](building-hmm-model), _[HMM3 search](searching-sequence-using-hmm-profile),_ and [_Phmmer search_](searching-sequence-against-sequence-database).

In the original program, the corresponding commands are: “hmmbuild”, “hmmsearch” and “phmmer”.

To access these tools select the _Tools ‣ HMMER tools_ submenu of the program main menu:


![](/images/54363788/56852533.png)

We highly recommend reading the original HMMER3 documentation to learn how to use utilities provided by the plugin.
