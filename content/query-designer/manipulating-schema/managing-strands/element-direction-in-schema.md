---
title: "Element Direction in Schema"
weight: 1
---


# Element Direction in Schema

For some _algorithm elements_ (e.g. _ORF_) the _Direction_ parameter is available in the _Property Editor_. It specifies the direction of the current element relatively to other elements in the schema and can take the following values:

*   _Direct_ — specifies to search the results for the element in the current strand.
*   _Forward_ — specifiesd to search the results for the element in the reverse complementary strand.
*   _Any_ — the results for the element are seached in the both strands.

Notice that an element changes it’s appearance on the _Scene_ when different values are selected:


![](/images/65930647/65930648.png)

**Example1:**

Create the following schema:

1.  The Smith-Waterman _algorithm element_ with _AAG_ patern and the _Forward_ direction.
2.  The Smith-Waterman element with _CGG_ pattern and the _Backward_ direction.
3.  Add a _constraint_ to these elements.
4.  Run the schema for a sequence.

By default, if the _Query Sequence Mode_ hasn’t been _modified_, the followings results will be found:


![](/images/65930647/65930649.png)

and


![](/images/65930647/65930650.png)
