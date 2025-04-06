---
title: "Metainformation Query Designer Element"
weight: 1
---


# Metainformation Query Designer Element

The metainformation is added when you create / edit the schema with the _Query Designer_. It is not required for running the schema and is skipped when the schema is created manually, for example:

#Open Reading Frame surrounded by repeat units

query ORF-Repeats {

    Repeat {
        type: repeats;
        min-length: 10;
    }

    ORF { type: orf; }

    Repeat.left--ORF.unit {
        type: distance;
        distance\_type:
        end-to-start;
        min: 0;
        max: 5000;
    }
    ORF.unit--Repeat.right {
        type: distance;
        distance\_type: end-to-start;
        min: 0;
        max: 5000;
    }
}
