---
title: "Querying Sequence Strands"
weight: 200
---

# Querying Sequence Strands

As the **Example1** above shows, both sequence strands are queried by default.

To modify this behavior, select the _Actions ‣ Query Sequence Mode_ item in the main menu or the _Query Sequence Mode_ toolbar button. You can choose between the following options:

*   _Direct strand_ — the search is performed for the direct strand only.

    Note that the results can still be found in the complement strand if you have set the _Any_ or _Backward_ direction for an element.

*   _Reverse complementary strand_ — the search is performed for the reverse complementary strand.

*   _Both strands_ — the search is performed for both strands.

**Example2:**

Create the following schema:

1.  The Smith-Waterman _algorithm element_ with _AAG_ pattern and the _Forward_ direction.
2.  The Smith-Waterman element with _CGG_ pattern and the _Forward_ direction.
3.  Add a _constraint_ to these elements.
4.  Set the _Query Sequence Mode_ to _Direct strand_.
5.  Run the schema for a sequence.

Only the following results will be found:

![](/images/65930651/65930652.png)