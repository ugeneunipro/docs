---
title: "Dataflow"
weight: 1
---


# Dataflow

The description of the elements is followed by the description of their connections to each other, i.e. the dataflow. For ports connections the description starts with the **.actor-bindings** keyword and has the following format:

    .actor-bindings {
        element1\_name.output\_port1\_name->element2\_name.input\_port2\_name;
    }

This pair says that data from port_1_ of _element1_ will be transferred to _port2_ of _element2_. For slots the following format without start keyword is used:

element1\_name.slot1\_name->element2\_name.port2\_name.slot2\_name

This pair says that data from _slot1_ of _element1_ will be transferred to _slot2_ of _port2_ of _element2_. See, for example, the minimum description of a dataflow of a workflow, that aligns an input MSA and writes the result to a file in ClustalW format.

    .actor-bindings {
        read-msa.out-msa->muscle.in-msa
        muscle.out-msa->write-msa.in-msa
    }
    read-msa.msa->muscle.in-msa.msa
    muscle.msa->write-msa.in-msa.msa
