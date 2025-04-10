---
title: "Validating Workflow"
weight: 500
---

# Validating Workflow

Before a workflow can be executed, it should be verified by the Workflow Designer. During the verification process, the Workflow Designer checks for errors in the dataflow logic or unspecified parameters, and can provide users with optimization or layout hints. If no errors are found, the workflow is valid to be [_run_](running-workflow).

You can request workflow validation at any stage of the workflow design. To do so, choose the _Actions ‣ Validate workflow_ item in the main menu, use the _Validate workflow_ toolbar button, or invoke it by pressing Ctrl+E. A list of identified issues and warnings, if any, or a notification of validation success will appear.

![](/images/2097179/2359311.png)

Double-clicking on items in the list selects the faulty element or iteration.