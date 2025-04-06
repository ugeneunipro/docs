---
title: "Custom External Tools"
weight: 1
---


# Custom External Tools

A custom tool can be integrated into the UGENE GUI as a workflow element in the [Workflow Designer](https://local.ugene.unipro.ru/wiki/display/WDD33/About+the+Workflow+Designer) - a UGENE component that allows joining tools into workflows.

As described in the "[Custom Elements with External Tools](https://local.ugene.unipro.ru/wiki/display/WDD33/Custom+Elements+with+External+Tools)" chapter of the Workflow Designer documentation, there are two options when one creates such workflow element:

*   Set a local executable path
*   Set an integrated external tool

The first option is intended for cases when a quick temporary integration of a tool into a workflow is enough.

The second option, although requires additional configuration steps, provides a more close integration with UGENE. It can be used by advanced UGENE users for providing a tool for their colleagues.

Below the preparatory configuration steps for the second option are described.

### Create an XML configuration file for custom external tool

Create an XML file with the custom external tool description. The file should match the following XML schema:

<?xml version = "1.0" encoding = "UTF-8"?>
<xs:schema xmlns:xs = "http://www.w3.org/2001/XMLSchema">

<xs:element name = "ugeneExternalToolConfig">
    <xs:complexType>
        <xs:sequence>
            <xs:element name = "name" type = "xs:string" />
            <xs:element name = "id" type = "xs:string" />
            <xs:element name = "executableName" type = "xs:string" />
            <xs:element name = "executableFullPath" type = "xs:string" minOccurs ="0" />
            <xs:element name = "description" type = "xs:string" minOccurs ="0" />
            <xs:element name = "version" type = "xs:string" minOccurs ="0" />
            <xs:element name = "launcherId" type = "xs:string" minOccurs ="0" />
            <xs:element name = "dependencies" type = "xs:string" minOccurs ="0" />
        </xs:sequence>
        <xs:attribute name = "version" type = "xs:string" use="required" />
    </xs:complexType>
</xs:element>

</xs:schema>

There XML elements have the following meaning:

*   **name** - the external tool name as it should be displayed in the UGENE GUI. This XML element is mandatory.
*   **id** - the external tool unique identifier. The following characters are allowed: letters ('A'-'Z'), digits ('0'-'9), '\_', '-'. This XML element is mandatory.
*   **executableName** - the name of the tool executable file (with the file extension, if it is present). This XML element is mandatory.
*   **executableFullPath** - a full path to the external tool executable. This XML element is optional. If the "executableFullPath" value is not specified, UGENE searches for a file with the specified "executableName" name in the same folder as the XML config file and sets the tool path accordingly. One can also specify either an absolute path to a file or a path, relative to the XML config. The path is displayed near the tool in the "Application Settings" dialog. It can be also manually set up by a user.
*   **description** - a detailed description of the external tool. This XML element is optional.
*   **version** - a version of the tool executable. This XML element is optional.
*   **launcherId** - if the tool is supposed to be run with some script interpreter or it is a java application, then this element should contain an appropriate ID. Currently, UGENE supports the following launchers IDs: **USUPP\_PYTHON2**, **USUPP\_PERL**, **USUPP\_RSCRIPT**, **USUPP\_JAVA**. If the launcher is specified, it would be added to the launch command explicitly whenever you try to launch the external tool. The path to the launcher will be taken from the "Application Settings" (see the corresponding tools in the "Supported tools" group). If the element is not specified or it is empty, no additional launcher will be added to the command that will run the tool. This XML element is optional.

*   **dependencies** - a comma-separated list of other external tool IDs the new tool is dependent from. If the dependency is not satisfied, then the dependent tool is marked as "not valid" in UGENE. This XML element is optional.


See also the following examples:

*   A minimalistic config:

    <?xml version = "1.0" encoding = "UTF-8"?>
    <ugeneExternalToolConfig version = "1.0">
        <name>An imported custom tool</name>
        <id>CUSTOM\_TOOL</id>
        <executableName>my\_tool.py</executableName>
    </ugeneExternalToolConfig>

    This config describes only the tool name, the tool ID and the tool executable file path. If the XML config is imported from the same folder as the python script, the path will be set to the python script. The tool won't have any dependencies, its version will be "unknown".

*   A config without dependencies and a launcher:

    <?xml version = "1.0" encoding = "UTF-8"?>
    <ugeneExternalToolConfig version = "1.0">
        <name>RAxML</name>
        <id>RAXML</id>
        <executableName>raxmlHPC</executableName>
        <executableFullPath>./my\_folder/raxmlHPC</executableFullPath>
        <description>RAxML - Randomized Axelerated Maximum Likelihood</description>
        <version>8.2.12</version>
    </ugeneExternalToolConfig>

    This config describes an external tool with a description and a version. Path to the tool executable is relative: it is supposed that the folder structure is the following:

    my\_config.xml
    my\_folder/
       raxmlHPC

*   A config with a dependency and a launcher:

    <?xml version = "1.0" encoding = "UTF-8"?>
    <ugeneExternalToolConfig version = "1.0">
        <name>HISAT2</name>
        <id>HISAT2</id>
        <executableName>hisat2</executableName>
        <executableFullPath>d:\\work\\hisat2.1\\hisat2<executableFullPath>
        <description>HISAT2 is a fast and sensitive alignment program for
    mapping next-generation sequencing reads (both DNA and RNA) to a
    population of human genomes (as well as to a single reference genome).</description>
        <toolkitName>HISAT2</toolkitName>
        <version>2.1.0</version>
        <launcherId>UGENE\_PERL</launcherId>
        <dependencies>UGENE\_PERL</dependencies>
    </ugeneExternalToolConfig>

    This config describes a tool that is supposed to be run by the Perl interpreter. There is no Perl by default on Windows, but the UGENE installer provides a possibility to install Perl. The tool can notify UGENE that it should be launched by Perl, so UGENE will add a path to Perl to the command that runs the tool. The XML config also specifies an absolute full path to the executable file.


### Prepare a package with the XML configuration file, the tool executable and, optionally, other files

The easiest way to "pack" the custom external tool is to:

*   create a new folder with all files required for running the tool,
*   specify a relative path in the XML configuration file described above,
*   put the XML configuration file into the same folder as the main tool executable.

This "package" can be shared with other users, if required.

### Import the tool into UGENE

To add the custom external tool one needs to import its XML configuration file in the "Custom tools" group on the "External Tools" page of the "Application Settings" dialog.
