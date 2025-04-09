---
title: "Filter BAM SAM Files Element"
weight: 800
---

# Filter BAM SAM Files Element

Filters BAM/SAM files using SAMTools view.

**Element type:** `filter-bam`

---

## Parameters

| **Parameter**  | **Description**                                                                                                                                                    | **Default Value** | **Parameter in Workflow File** | **Type**  |
|----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------------------------------|-----------|
| Output folder  | Select an output directory. Custom – specify the output directory in the 'Custom directory' parameter. Workflow – internal workflow dir. Input file – use its dir. | *(none)*          | `out-mode`                     | _numeric_ |
| Output name    | Name of an output BAM/SAM file. If empty, uses the name of the first input file with `.filtered` extension.                                                        | *(none)*          | `out-name`                     | _string_  |
| Output format  | Format of the output assembly file.                                                                                                                                | `bam`             | `out-format`                   | _string_  |
| Region         | Regions to filter (BAM only). Example: `chr2`, `chr2:1000`, or `chr2:1000-2000`. Multiple regions separated by space.                                              | *(none)*          | `region`                       | _string_  |
| MAPQ threshold | Minimum MAPQ quality score.                                                                                                                                        | `0`               | `mapq`                         | _numeric_ |
| Accept flag    | Output alignments matching selected flags. Leave empty to skip this filter.                                                                                        | *(none)*          | `accept-flag`                  | _string_  |
| Skip flag      | Skip alignments matching selected flags. Leave empty to skip this filter.                                                                                          | *(none)*          | `flag`                         | _string_  |

---

## Input/Output Ports

### Input Port

- **Name in GUI:** `BAM/SAM File`
- **Name in Workflow File:** `in-file`

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| Source URL  | `input-url`           | _string_ |

### Output Port

- **Name in GUI:** `Filtered BAM/SAM files`
- **Name in Workflow File:** `out-file`

| Slot In GUI | Slot in Workflow File | Type     |
|-------------|-----------------------|----------|
| Source URL  | `output-url`          | _string_ |
