---
title: "Export Sequences Associated with Annotation"
weight: 500
---

# Export Sequences Associated with Annotation

In UGENE you can export a sequence associated with an annotation. To do this, select the annotation in the _Project View_ window and click the _Export/Import‣ Export corresponding sequence_ option in the context menu:

![](/images/65929318/65929319.png)

The _Export Selected Sequences_ dialog will appear:

![](/images/65929318/96665855.png)

Here you can select the location of the result file and a sequence file format. You can choose to add the newly created document to the current project and use a custom sequence name. To do this, check the corresponding checkboxes.

Use the _Conversion options_ to choose a strand for saving sequence(s). Additionally, you can translate sequence(s) to an amino alphabet.

It is also possible to specify whether to merge the exported sequences into a single sequence or store them as separate sequences. If you merge the sequences, you're allowed to select the gap symbols between sequences. This defines the length of the insertion region between sequences that contain **N** symbols for nucleic or **X** for protein sequences.

#### Export sequence with annotations

To export a sequence with annotations, choose the Genbank or GFF format. The _Export with annotations_ checkbox will be available. Check the checkbox, and the sequence will be exported with annotations.