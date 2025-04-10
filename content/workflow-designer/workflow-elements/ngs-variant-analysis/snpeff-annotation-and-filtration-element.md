---
title: "SnpEff Annotation and Filtration Element"
weight: 500
---

# SnpEff Annotation and Filtration Element

Annotates and filters variations with SnpEff.

**Element type:** seff

Parameters
----------

| Parameter                     | Description                                                                                                                                                                                                   | Default value                                | Parameter in Workflow File | Type     |
|-------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------|-----------------------------|----------|
| **Output directory**          | Select an output directory. Custom - specify the output directory in the 'Custom directory' parameter. Workflow - internal workflow directory. Input file - the directory of the input file.                    | Input file                                   |                                 |          |
| **out-mode**                  |                                                                                                                                                                                                               |                                              | _string_                        | _string_ |
| **Input format**              | Select the input format of variations.                                                                                                                                                                       | VCF                                          | **inp-format**                | _string_ |
| **Output format**             | Select the format of annotated output files.                                                                                                                                                                  | VCF                                          | **out-format**                | _string_ |
| **Genome**                    | Select the target genome from the list of SnpEff databases. Genome data will be downloaded if it is not found. The list of databases depends on the SnpEff external tool version.                              | Homo sapiens                                 | **genome**                   | _string_ |
| **Upstream/downstream length**| Upstream and downstream interval size. Eliminate any upstream and downstream effects by using 0 length.                                                                                                      | No upstream/downstream interval (0 bases)    | **updown-length**            | _numeric_|
| **Canonical transcripts**     | Use only canonical transcripts.                                                                                                                                                                             | False                                        | **canon**                    | _boolean_|
| **HGVS nomenclature**         | Annotate using HGVS nomenclature.                                                                                                                                                                           | False                                        | **hgvs**                     | _boolean_|
| **Annotate loss of function** | Annotate Loss of function (LOF) and Nonsense-mediated decay (NMD).                                                                                                                                           | False                                        | **lof**                      | _boolean_|
| **Annotate TFBSs motifs**     | Annotate transcription factor binding site motifs (only available for the latest GRCh37).                                                                                                                   | False                                        | **motif**                    | _boolean_|

Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** Variations

**Name in Workflow File:** in-file

**Slots:**

| Slot In GUI | Slot in Workflow File | Type    |
|-------------|------------------------|---------|
| **Source url** | **url**                 | _string_ |

And 1 _output port_:

**Name in GUI:** Annotated variations

**Name in Workflow File:** out-file

**Slots:**

| Slot In GUI | Slot in Workflow File | Type       |
|-------------|------------------------|------------|
| **Source url** | **url**                 | _variation_ |

