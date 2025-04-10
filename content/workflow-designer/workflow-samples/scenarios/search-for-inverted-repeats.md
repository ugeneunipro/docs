---
title: "Search for Inverted Repeats"
weight: 200
---

# Search for Inverted Repeats

For each input sequence, the workflow performs a search for inverted repeats.

It then saves the repeats found on the direct strand to the "direct\_strand\_repeat\_units.fa" file and the complementary ones to the "compl\_strand\_repeat\_units.fa" file.

How to Use This Sample

If you haven't used the workflow samples in UGENE before, please look at the "[How to Use Sample Workflows](../../introduction/how-to-use-sample-workflows)" section of the documentation.

##### Workflow Sample Location

The workflow sample "Search for Inverted Repeats" can be found in the "Scenarios" section of the Workflow Designer samples.

##### Workflow Image

The opened workflow looks as follows:

![](/images/65930535/65930536.png)

##### Workflow Wizard

The wizard has 3 pages.

1. **Input sequence(s):** On this page, you must input sequence(s).


    ![](/images/65930535/65930537.png)

2. **Search for inverted repeats parameters:** On this page, you can modify inverted repeats parameters.


    ![](/images/65930535/65930538.png)

    The following parameters are available:

    - **Annotate as:** Name of the result annotations marking found repeats.
    - **Min length:** Minimum length of repeats.
    - **Identity:** Repeats identity.
    - **Min distance:** Minimum distance between repeats.
    - **Max distance:** Maximum distance between repeats.
    - **Filter algorithm:** Filter repeats algorithm.
    - **Algorithm:** Control over variations of the algorithm.
    - **Parallel threads:** Number of parallel threads used for the task.

3. **Output Sequences:** On this page, you can modify result file(s) settings.


    ![](/images/65930535/65930539.png)