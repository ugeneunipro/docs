---
title: "UGENE Command Line Interface"
weight: 1400
---

# UGENE Command Line Interface

The UGENE command line interface (CLI) was developed with the following principles in mind:

* To make it as easy to use as popular shell commands.
* To include all significant UGENE features.
* To allow users to add their own commands.

To use the UGENE CLI, ensure that you add the path to the UGENE executable to your **%PATH%** environment variable.

The general syntax is as follows:

```
ugene [[--task=]task_name] [--task_parameter=value ...] [-task_parameter value ...] [--option[=value]] [-option[ value]]
```

Here:

**task_name** — The task to execute, which can be one of the [_predefined tasks_](cli-predefined-tasks.md) or [_a task you have created_](creating-custom-cli-tasks).

**task_parameter** — A parameter of the specified task. Some parameters of a task are required, such as the _in_ and _out_ parameters of some tasks.

**option** — One of the [_CLI options_](cli-options).

See the example below:

```
ugene align --in=COI.aln -out result.aln -log-level-details