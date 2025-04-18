---
title: "Read Sequence from Remote Database Element"
weight: 900
---

# Read Sequence from Remote Database Element

Download sequence(s) with the specified ID(s) from one of the remote databases: NCBI, Ensembl, PDB, etc.

The sequences are downloaded with the associated annotations in a file format specific to the selected database.

The element outputs message(s) with the sequence and annotations data.

**Element type:** fetch-sequence

## Parameters

| Parameter                       | Description                                                     | Default Value               | Parameter in Workflow File | Type     |
|---------------------------------|-----------------------------------------------------------------|-----------------------------|-----------------------------|----------|
| **Resource IDs** (required)     | Semicolon-separated list of resource IDs in the database.       |                             | **resource-id**             | _string_ |
| **Database** (required)         | Name of the database to read from.                              | NCBI Genbank (DNA sequence) | **database**                | _string_ |
|                                 | Available values are:                                           |                             |                             |          |
|                                 | - ncbi-dna (NCBI GenBank (DNA sequence))                        |                             |                             |          |
|                                 | - ncbi-protein (NCBI protein sequence database)                 |                             |                             |          |
|                                 | - pdb (PDB)                                                    |                             |                             |          |
|                                 | - swiss-plot (SWISS-PROT)                                       |                             |                             |          |
|                                 | - uniprot-swiss-prot (UniProtKB/Swiss-Prot)                     |                             |                             |          |
|                                 | - uniprot-trembl (UniProtKB/TrEMBL)                             |                             |                             |          |
| **Save file to directory**      | Directory to store a file loaded from the database.             | default                     | **save-dir**                | _string_ |
| **Read resource ID(s) from source** | The source to read resource IDs from the list or a local file. | List of TDs                 | **ids-source**              | _string_ |

## Input/Output Ports

The element has 1 _output port_:

| Name in GUI   | Name in Workflow File | Type              |
|---------------|-----------------------|-------------------|
| **Sequence**  | out-sequence          | _sequence_        |
| **Set of annotations** | annotations            | _annotation-table_ |