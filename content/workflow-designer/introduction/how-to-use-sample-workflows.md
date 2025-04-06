---
title: "How to Use Sample Workflows"
weight: 1
---


# How to Use Sample Workflows

[UGENE Workflow Designer](about-the-workflow-designer.md) contains a set of sample workflows that help a biologist to solve certain tasks for multiple input files or datasets at the same time. The list of samples can be found in the [Workflow Samples section](workflow-samples.md) of the documentation.

To use a sample:

1.  Start the Workflow Designer by selecting "Tools > Workflow Designer" in the main menu of the UGENE window.
    _See also:_ [the paragraph about launching the Workflow Designer](launching-workflow-designer.md).


2.  Select the "Samples" tab on the [Workflow Designer palette](workflow-designer-window-components.md), i.e. on the left side of the opened window.
    _See also:_ the tab is described in the [Workflow Samples section](workflow-samples.md).


3.  Double-click on the required sample.
    The workflow will be opened and shown on the [Workflow Designer scene](workflow-designer-window-components.md), i.e. the center area of the window.
    For example, a workflow for doing BLAST and getting the results from the NCBI server is shown below.


    ![](/images/11763719/11862017.png)



4.  Select the wizard button on the Workflow Designer toolbar (the button is marked on the image below) to start the wizard for the workflow.
    _Additional technical details:_ A wizard can be used to configure all the parameters for the workflow more easily. The other way to configure the parameters is by editing them in the [Property Editor](workflow-designer-window-components.md). A wizard is not available for a newly created workflow, but it can be added by editing the workflow file.


    ![](/images/11763719/11862039.png)

5.  Input the required data. The input varies very much on the workflow that has been selected on step 3 (see above).
    For example, in case of the remote BLAST workflow, at least one sequence is expected to be input. On the image below two sequences were input for the workflow. Buttons that can be used to add different files or even folders with files are also marked on the image.


    ![](/images/11763719/11862040.png)



6.  Optionally, modify the workflow parameters on other pages of the wizard.


7.  Click the "Run" button on the last wizard page to run the workflow.
    For example:



    ![](/images/11763719/11862041.png)



8.  Launching of the workflow opens the dashboard. Wait until the workflow is finished. The output files will be available in the corresponding section of the dashboard.
    For example, in case of the remote BLAST workflow, the dashboard will look as follows:


    ![](/images/11763719/11862042.png)
