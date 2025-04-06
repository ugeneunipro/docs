---
title: "How to open and save intermediate breakpoint results"
weight: 1
---


# How to open and save intermediate breakpoint results

During debugging, it is sometimes necessary to view the intermediate results after each step.

For this purpose, the table "Messages from <worker1> to <worker2>" is provided. The "Process one message" and "Next" buttons are required to fill this table.

Let's look at this with at the workflow example: "Samples"- >"Alignment"->"Align sequences with MUSCLE".

*   Select   "Read Alignment" worker and add input files "COI.aln" and "HIV-1.aln" from data/samples/CLUSTALW.
*   Set a breakpoint on the "Align with MUSCLE" element from context menu or Ctrl+B shortcut.
    The "Align with MUSCLE" element has a red frame.
*   Press Ctrl+R  (Run workflow). The breakpoint was triggered.




![](/images/116293679/116293704.png)

      At first click on the connection between the "Align with MUSCLE" and "Write alignment" elements.
      An empty table "Messages from 'Align with MUSCLE' to 'Write alignment'" appears.
      Note, that "Process one message" button on the main toolbar is disabled.


![](/images/116293679/116293705.png)

     Select the "Read alignment" element on the Scene.
     After that action "Process one message" button on the main toolbar become enabled.

    Click "Process one message".   A new row appears in the intermediate table.




![](/images/116293679/116293706.png)

The value from this table we can Convert to document or Copy to clipboard from context menu.
