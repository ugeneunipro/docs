---
title: "Creating Annotation"
weight: 100
---


# Creating Annotation

To create a new annotation for the active sequence press the Ctrl-N key sequence, select the _New annotation_ toolbar button, or use the _Add ‣ New annotation_ or _New annotation_ context menu item:


![](/images/65929465/82608245.png)

This will activate a dialog where to set up annotation parameters:


![](/images/65929465/65929466.png)

The dialog asks where to save the annotation. It could be either an existing annotation table object or an a new annotation table.

You can also specify the name of the group and the name of the annotation. If the group name is set to <auto> UGENE will use the group name as the name for the group. You can use the ‘/’ characters in this field as a group name separator to create subgroups. If the annotation name is set to _by type_ UGENE will use the annotation type from the _Annotation type:_ table as the name for the annotation. Also, you can add a description in the corresponding text field.

The _Location_ field contains annotation coordinates. The coordinates must be provided in the Genbank or EMBL file formats. If you want to annotate complement strand sequence check the corresponding checkbox for the simple format or surround the coordinates with the “complement()” word or press the last button in the corresponding row to do it automatically.

Note, that by default the _Location_ field contains the coordinates of the selected sequence region.


For amino acid sequences there is no "Complement" check box in the "Simple format" group in the Location section and there is no "Add/remove complement flag" button in the "GenBank/EMBL format" group.


![](/images/65929465/65929468.png)



Once the _Create_ button is pressed the annotation is created and highlighted both in the _Sequence overview_ and the _Sequence details view_ areas:


![](/images/65929465/82608246.png)
