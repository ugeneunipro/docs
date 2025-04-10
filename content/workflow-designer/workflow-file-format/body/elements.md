---
title: "Elements"
weight: 100
---

# Elements

Each _element_ used in the _workflow_ must be described within the body. An element description consists of the element name and a set of parameters enclosed in curly braces. A parameter and its value are separated by a colon ‘:’, and different parameters are separated by semicolons ‘;’:

```
element_name {
    parameter1:value1;
    parameter2:value2;
    ...
}
```

See, for example, a description of the [_Read alignment_](../../workflow-elements/data-readers/read-alignment-element) element:

```
read-msa {
    type:read-msa;
    name:"Read alignment";
    url-in:/home/user/pkinase.sto;
}
```

Note that the values of the parameters for an element can also be presented in the [_iterations_](/wiki/pages/createpage.action?spaceKey=WDD34&title=Using+Iterations) block. For all elements, the following parameters are defined:

- **type** - specifies the type of the element.
- **name** - specifies the name of the element. It corresponds to the element’s name in the GUI.
- **.validator** - validates the element using the input validator type's parameters:
  - **type** - specifies the type of the validator.

For example, this validator ensures that the read sequence element has two or three datasets:

```
read-sequence {
    type:read-sequence;
    name:"Read Sequence";
    .validator {
        type:datasets-count;
        min:2;
        max:3;
    }
}
```

For _custom elements_, there is a special parameter:

- **script** - sets the script text of the element, for example:

```
dump-info {
    type:"Script-Dump sequence info";
    name:"Dump sequence info";
    script {
        out_text=getName(in_sequence) + ": " + size(in_sequence);
    }
}
```

The list of available parameters depends on the element. Refer to the [_Workflow Elements_](workflow-elements.md) chapter to find out the parameters for a particular element. To [_set a script value for a parameter_](../../using-script-to-set-parameter-value), use the following form:

```
parameter_name {
    a script value
};