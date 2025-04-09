---
title: "CD-Search Element"
weight: 300
---

# CD-Search Element

Finds conserved domains in protein sequences.
If the conserved domains database is downloaded, the search can be executed locally.
Otherwise, the search can be submitted to the NCBI for remote execution.

**Element type:** cd-search

## Parameters

| Parameter              | Description                                                                                                                                                                                                                                                                                                                                                                  | Default value | Parameter in Workflow File | Type      |
|------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------|-----------|
| **Annotate as**        | Name of the result annotations marking found conserved domains.                                                                                                                                                                                                                                                                                                              | CDD result    | **result-name**            | _string_  |
| **Database**           | CD-Search is offered with the following databases: <br><br>• **CDD** – superset including curated and imported domains<br>• **Pfam** – curated seed alignments<br>• **SMART** – domain alignments, some limitations<br>• **TIGRFAM** – curated HMM alignments<br>• **COG** – orthologous protein families<br>• **KOG** – eukaryotic orthologs<br>• **Prk** – protein kinases | CDD           | **db-name**                | _string_  |
| **Database directory** | Specifies path to local copy of the database used for local search.                                                                                                                                                                                                                                                                                                          |               | **db-path**                | _string_  |
| **Local search**       | If `True`, performs search locally. If `False`, submits query to NCBI for remote execution.                                                                                                                                                                                                                                                                                  | True          | **local-search**           | _boolean_ |
| **Expect value**       | Modifies the [E-value](http://www.ncbi.nlm.nih.gov/BLAST/blastcgihelp.shtml#expect) threshold for filtering results. A typical cutoff is 0.01. Results with E-values > 1 are usually considered unreliable.                                                                                                                                                                  |               | **e-val**                  | _numeric_ |

## Input/Output Ports

| Port Name (GUI)    | Workflow File Name | Slots                                                       |
|--------------------|--------------------|-------------------------------------------------------------|
| **Input sequence** | `in-sequence`      | **Sequence** → `sequence` (_sequence_)                      |
| **Annotations**    | `out-annotations`  | **Set of annotations** → `annotations` (_annotation-table_) |
