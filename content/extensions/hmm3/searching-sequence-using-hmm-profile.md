---
title: "Sequence Search Using HMM Profile"
weight: 200
---

# Sequence Search Using HMM Profile

The _HMM3 search_ tool reads an HMM profile from a file and searches a sequence for significantly similar sequence matches.

The sequence must be selected in the _Project View_, or there must be an active _Sequence View_ window opened.

If the selected sequence is nucleic and the profile HMM is built from an amino acid alignment, the sequence will be automatically translated and searched in all possible frames (total of 6).

If a profile HMM is built for nucleotide alignment, the search is performed for both strands (direct and complement).

The _HMM3 search_ accepts the HMMER2 HMM profiles (amino acid only) as a backward compatibility feature. An interesting post about using the HMMER2 models with the HMMER3 is available on [Sean Eddy’s blog](http://selab.janelia.org/people/eddys/blog/?p=117).

![](/images/65930823/65930824.png)

For example, reporting threshold options can be configured using the dialog:

![](/images/65930823/65930825.png)

The search results are stored as sequence annotations in the GenBank file format.

![](/images/65930823/65930826.png)

The [_HMM3 search_](http://ugene.unipro.ru/documentation/manual/plugins/hmm3.html#hmm3-search) works only with files that contain a single HMM model.