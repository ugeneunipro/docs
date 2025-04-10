---
title: "Dataflow"
weight: 200
---


# Dataflow

The description of the elements is followed by the explanation of their connections to each other, i.e., the data flow. For port connections, the description starts with the **.actor-bindings** keyword and has the following format:

```plaintext
.actor-bindings {
    element1_name.output_port1_name->element2_name.input_port2_name;
}
```

This pair indicates that data from _port1_ of _element1_ will be transferred to _port2_ of _element2_. For slots, the following format without a start keyword is used:

```plaintext
element1_name.slot1_name->element2_name.port2_name.slot2_name
```

This pair indicates that data from _slot1_ of _element1_ will be transferred to _slot2_ of _port2_ of _element2_. See, for example, the minimum description of a data flow of a workflow that aligns an input MSA and writes the result to a file in ClustalW format.

```plaintext
.actor-bindings {
    read-msa.out-msa->muscle.in-msa
    muscle.out-msa->write-msa.in-msa
}
```

```plaintext
read-msa.msa->muscle.in-msa.msa
muscle.msa->write-msa.in-msa.msa