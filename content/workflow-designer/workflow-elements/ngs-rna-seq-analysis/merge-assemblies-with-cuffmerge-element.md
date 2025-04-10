---
title: "Merge Assemblies with Cuffmerge Element"
weight: 400
---

# Merge Assemblies with Cuffmerge Element

Cuffmerge merges several assemblies together. It also handles running Cuffcompare for you and automatically filters out a number of transfrags that are probably artifacts. If you have a reference file available, you can provide it to Cuffmerge to seamlessly merge input (e.g., novel) isoforms with known isoforms and maximize overall assembly quality.

**Element type:** cuffmerge

Parameters
----------

| Parameter                  | Description                                                                                                                         | Default value | Parameter in Workflow File   | Type  |
|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------------|-------|
| **Output directory**       | Directory to save MACS output files.                                                                                               |               | **out-dir**                  | _string_  |
| **Reference annotation**   | Merge the input assemblies together with this reference annotation.                                                                |               | **ref-annotation**           | _string_  |
| **Reference sequence**     | The genomic DNA sequences for the reference. It is used to assist in classifying transfrags and excluding artifacts (e.g., repeats). For example, transcripts consisting mostly of lowercase bases are classified as repeats. |               | **ref-seq**                  | _string_  |
| **Minimum isoform fraction** | Discard isoforms with abundance below this.                                                                                       | 0.05          | **min-isoform-fraction**     | _numeric_ |
| **Cuffcompare tool path**  | The path to the Cuffcompare external tool in UGENE.                                                                                | default       | **cuffcompare-tool-path**    | _string_  |
| **Cuffmerge tool path**    | The path to the Cuffmerge external tool in UGENE.                                                                                  | default       | **path**                     | _string_  |
| **Temporary directory**    | The directory for temporary files.                                                                                                 | default       | **tmp-dir**                  | _string_  |

Input/Output Ports
------------------

The element has 1 _input port_:

- **Name in GUI:** Set of annotations
- **Name in Workflow File:** in-assembly

**Slots:**

| Slot In GUI         | Slot in Workflow File | Type      |
|---------------------|-----------------------|-----------|
| **Set of annotations** | **in-annotations**  | _ann_table_ |

And 1 _output port_:

- **Name in GUI:** Set of annotations
- **Name in Workflow File:** out-assembly

**Slots:**

| Slot In GUI         | Slot in Workflow File | Type      |
|---------------------|-----------------------|-----------|
| **Set of annotations** | **out-annotations** | _ann_table_ |