---
title: "Fetching Sequence from Remote Database"
weight: 2500
---


# Fetching Sequence from Remote Database

**Task Name:** fetch-sequence

Fetches a sequence from a remote database. The supported databases are accesed via alias.

Database

Alias

NCBI Genbank (DNA)

genbank

NCBI Genbank (protein)

genbank-protein

Protein Data Bank

pdb

SwissProt

swissprot

Uniprot

uniprot

**Parameters:**

_db_ — database alias to read from. \[String, Required\]

_id_ — semicolon-separated list of resource IDs in the database. \[String, Required\]

_save-dir_ — directory to store sequence files loaded from the database. \[String, Optional\]

**Example:**

ugene fetch-sequence --db=PDB --id=3INS;1CRN
