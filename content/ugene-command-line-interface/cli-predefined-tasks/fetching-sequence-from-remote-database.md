---
title: "Fetching Sequence from Remote Database"
weight: 2500
---

# Fetching Sequence from Remote Database

**Task Name:** `fetch-sequence`

Fetches a sequence from a remote database. The supported databases are accessed via alias.

---

## Supported Databases

| **Database**           | **Alias**         |
|------------------------|-------------------|
| NCBI Genbank (DNA)     | `genbank`         |
| NCBI Genbank (protein) | `genbank-protein` |
| Protein Data Bank      | `pdb`             |
| SwissProt              | `swissprot`       |
| UniProt                | `uniprot`         |

---

## Parameters

- **`--db`** — Database alias to read from.
  _Type: `String`, Required._

- **`--id`** — Semicolon-separated list of resource IDs in the database.
  _Type: `String`, Required._

- **`--save-dir`** — Directory to store sequence files loaded from the database.
  _Type: `String`, Optional._

---

## Example

```bash
ugene fetch-sequence --db=PDB --id=3INS;1CRN
```
