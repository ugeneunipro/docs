---
title: "Searching Sequence Against Sequence Database"
weight: 300
---


# Searching Sequence Against Sequence Database

The _Phmmer search_ tool searches for query sequence matches in sequence database, much as BLASTP or FASTA would do.

The _Phmmer search_ works essentially like the _HMM3 search_ does, except you provide a query sequence instead of a query profile HMM.

The database sequence must be selected in the _Project View_ or there must be an active _Sequence View_ window opened.

Select the query sequence in the _Phmmer search_ dialog:


![](/images/65930828/65930829.png)

You can set options of the _Phmmer search_ by choosing the needed dialog tab. Here you can see the e-value calibration options:


![](/images/65930828/65930830.png)

The results are stored as sequence annotations in the Genbank file format.


![](/images/65930828/65930831.png)

The [_Phmmer search_](http://ugene.unipro.ru/documentation/manual/plugins/hmm3.html#phmmer) works only with single-sequence databases.
