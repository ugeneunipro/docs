---
title: "Metainformation"
weight: 300
---


# Metainformation

A metainformation block sets visual parameters of the workflow and aliases for running it from the command line.

Each block starts with **.meta** keyword and consists of the aliases and visual blocks:

.meta {
    aliases {
        # The workflow aliases
    }
    visual {
        # Visual data for element1
        # Visual data for element2
        # ...
    }
}

Parameter Aliases
-----------------

The block starts with the **parameter-aliases** keyword and has the following format:

parameter-aliases {
    element\_name.parameter\_name:value;
    ...
}

The value specified for an element parameter is used as the alias for this parameter when the workflow is [_executed from the command line_](../../running-workflow-from-the-command-line).

See an example of setting workflow aliases:

.meta {
    parameter-aliases {
        read-msa.url-in:in;
        write-msa.url-out:out;
    }
    ...
}

Visual

The block starts with the **visual** keyword. It describes the appearance of the workflow in a Workflow Designer window, i.e. appearance of the workflow _elements_ and _connections_:

visual {

    # Elements appearance
    element\_name1 {
        element\_appearance\_parameter1:value1;
        element\_appearance\_parameter2:value2;
        ...
    }
    element\_name2 {
        ...
    }
    ...


    # Connections appearance
    element1\_name.port1\_name->element2\_name.port2\_name {
        connection\_appearance\_parameter1:value3;
        ...
    }
    ...
}

To describe an element appearance the following parameters are used:

*   **description** — description of the element in the _Property Editor_. It is in HTML format.

*   **tooltip** — tooltip shown on the element.

*   **pos** — position of the element, assuming that bottom right corner of the window is (0, 0) position.

*   **style** — style of the element. The following values are available:

    *   **ext** — for extended element style
    *   **simple** — for minimal element style

*   ****bounds** —** defines the bounds of the element rectangle in the extended style.
*   **bg-color-ext** — color of the element in the extended style. The color must be specified in the RGBA format.
*   **bg-color-simple** — color of the element in the minimal style.
*   **port\_name.angle** — position of the port on the element. Here the _port\_name_ must be replaced by the name of the port.

For now, the only parameter that describes a connection appearance is:

*   **text-pos** — position of the text near the connection arrow.

For example:

visual {
    read-sequence {
        description:"";
        tooltip:"Reads sequences and annotations ...";
        pos:"-930 -885";
        style:ext;
        bg-color-ext:"0 128 128 64";
        bounds:"-30 -30 45 103";
        out-sequence.angle:272.309;
    }
    write-sequence {
        ...
    }
    read-sequence.out-sequence->write-sequence.in-sequence {
        text-pos:"-27.5 -24";
    }
