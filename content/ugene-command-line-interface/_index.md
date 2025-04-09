---
title: "UGENE Command Line Interface"
weight: 1400
---


# UGENE Command Line Interface

UGENE command line interface (CLI) was developed keeping in mind the following principles:

*   To make it as easy as popular shell commands.
*   To include all significant UGENE features.
*   To allow users to add their own commands.

To use UGENE CLI make sure to add the path to the UGENE executable to your **%PATH%** environment variable.

The general syntax is the following:

ugene \[\[--task=\]task\_name\] \[--task\_parameter=value ...\] \[-task\_parameter value ...\] \[--option\[=value\]\] \[-option\[ value\]\]

Here:

**task\_name** — task to execute, it can be one of the [_predefined tasks_](cli-predefined-tasks.md) or [_a task you have created_](creating-custom-cli-tasks.md).

**task\_parameter** — parameter of the specified task. Some parameters of a task are required, like _in_ and _out_ parameters of some tasks.

**option** — one of the [_CLI options_](cli-options.md).

See the example below:

ugene align --in=COI.aln -out result.aln -log-level-details
