---
title: "Creating Dotplot"
weight: 100
---


# Creating Dotplot

To create a dotplot select the _Tools ‣ Build dotplot_ main menu item. The _Build dotplot from sequences_ dialog will appear:


![](/images/65929583/65929584.png)

Here you should specify the _File with first sequence_. Also you should either check the _Compare sequence against itself_ option or select the _File with second sequence_.

Optionally you can select to _Join all sequences found in the file_ (for the first and/or for the second file). If you select to join the sequences you can also select the _Gap size_. The gap of the specified size will be inserted between the joined sequences.

After you press the _Next_ button, the dialog to configure the dotplot parameters will appear:


![](/images/65929583/65929585.png)

The following parameters are available:

_X axis sequence_ — the sequence for the X dotplot axis.

_Y axis sequence_ — the sequence for the Y dotplot axis.

If there are several sequences in the specified (the first or the second) file and you haven’t selected to join the sequences in the previous dialog, then you can select a sequence in these fields.

If you have selected to _Join all sequences found in the file_, then you can’t select a separate sequence from the file, the joined _Sequence_ can be selected instead.

_Search direct repeats_ — check this option to search for direct repeats in the specified sequences. You can also select the color with which the repeats will be displayed in the picture. The _default_ button sets the default color.

_Search inverted repeats_ — check this option to search for inverted repeats in the specified sequences. You can also select the color with which the repeats will be displayed in the picture. The _default_ button sets the default color.

_Custom algorithm_ — optionally you can select an algorithm to calculate the repeats:

*   Auto
*   Suffix index
*   Diagonals

The specified algorithm is provided to the [_Repeat Finder_](repeat-finder.md) plugin as an input parameter. In most cases the _Auto_ value is appropriate.

_Minimum repeat length_ — allows to draw only such matches between the sequences that are continuous and long enough. For example if it equals to _3bp_, then only repeats will be found that contain 3 and more base symbols.

Press the _1k_ button to automatically adjust the _Minimum repeat length_ value. Such value will be set, that there will be about 1000 repeats found.

_Repeats identity_ — specifies the percents of the repeats identity.

Press the _100_ button to set the _100%_ identity.

After the parameters are set, press the _OK_ button. The dotplot will appear in the _Sequence View_:


![](/images/65929583/65929586.png)

It is a two-dimentional plot consisted of dots.

Each dot on the plot corresponds to a matched base symbol at the “x” position of the horizontal sequence and the “y” position of the vertical sequence.

Visible diagonal lines indicate matches between sequences in the given particular region.

See also:

*   [_Interpreting Dotplot: Identifying Matches, Mutations, Invertions, etc._](65929597.html)
*   [_Building Dotplot for Currently Opened Sequence_](building-dotplot-for-currently-opened-sequence)
