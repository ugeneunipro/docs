---
title: "CLI Options"
weight: 100
---

# CLI Options

_\--help | -h \[<option\_name> | <task\_name>\]_

Shows help information. For example:

```shell
ugene --help                      ## Shows general UGENE CLI help.
ugene -h

ugene --help=<option_name>        ## Shows help for the <option_name> option.
ugene -h <option_name>

ugene --help=<task_name>          ## Shows help for the <task_name> task.
ugene -h <task_name>
```

_\--task=<task_name> \[<task_parameter>=value ...\]_

Specifies the task to run. A user-defined UGENE workflow schema can be used as a task name. For example:

```shell
ugene --task=align --in=COI.aln --out=result.aln

ugene --task=C:\myschema.uwl --in=COI.aln --out=res.aln
```

_\--log-no-task-progress_

A task progress is shown by default when a task is running. This option specifies not to show the progress.

_\--log-level="\[<category1>=\]<level1> \[, ...\]"_

Sets the log level per category. If a category is not specified, the log level is applied to all categories.

The following categories are available:

*   “Algorithms”
*   “Console”
*   “Core Services”
*   “Input/Output”
*   “Performance”
*   “Remote Service”
*   “Scripts”
*   “Tasks”

The following log levels are available: TRACE, DETAILS, INFO, ERROR, or NONE.

By default, loglevel=ERROR.

For example:

```shell
ugene --log-level=NONE

ugene --log-level="Tasks=DETAILS, Console=DETAILS"
```

_\--log-format="<format_string>"_

Specifies the format of a log line.

Use the following notations: L - level, C - category, YYYY or YY - year, MM - month, dd - day, hh - hour, mm - minutes, ss - seconds, zzz - milliseconds.

By default, logformat=”\[L\]\[hh:mm\]”.

_\--license_

Shows license information.

_\--lang=language_code_

Specifies the language to use (e.g., for the log output). The following values are available:

*   _CS_ (Czech)
*   _EN_ (English)
*   _RU_ (Russian)

_\--log-color-output_

If log output is enabled, this option makes it colored: _ERROR_ messages are displayed in red, _DETAILS_ messages are displayed in green, _TRACE_ messages are displayed in blue.

\--_session-db_

Session database is stored in the temporary file that is created for every UGENE run. But it can be supplied with the command line argument. If the supplied file does not exist, it will be created. The session database file is removed after closing UGENE.

For example:

```shell
ugene --session-db=D:/session.ugenedb
```

\--_version_

Shows version information.

\--_tmp-dir=<path_to_file>_

Path to temporary folder.

\--_ini-file=<path_to_file>_

Loads configuration from the specified .ini file. By default, the UGENE.ini file is used.

\--_genome-aligner_

UGENE Genome Aligner is an efficient and fast tool for short read alignment. It has two work modes: build index and align short reads (default mode). If there is no index available for the reference sequence, it will be built on the fly.

Usage: _ugene --genome-aligner { --option\[=argument\] }_

The following options are available:

* _\--build-index_ Use this flag to only build the index for the reference sequence.
* _\--reference_ Path to reference genome sequence
* _\--short-reads_ Path to short reads data in FASTA or FASTQ format
* _\--index_ Path to prebuilt index (base file name or with .idx extension). If not set, the index is searched in the system temporary directory. If --build-index option is applied, the index will be saved to the specified path.
* _\--result_ Path to output alignment in UGENEDB or SAM format (see --sam)
* _\--memsize_ Memory size (in MBs) reserved for short reads. The bigger the value, the faster the algorithm works. Default value depends on available system memory.
* _\--ref-size_ Index fragmentation size (in MBs). Small fragments better fit into RAM, allowing loading more short reads. Default value is 10.
* _\--n-mis_ Absolute amount of allowed mismatches per every short read (mutually exclusive with --pt-mis). Default value is 0.
* _\--pt-mis_ Percentage amount of allowed mismatches per every short read (mutually exclusive with --n-mis). Default value is 0.
* _\--rev-comp_ Use both the read and its reverse complement during the aligning.
* _\--best_ Report only the best alignments (in terms of mismatches).
* _\--omit-size_ Omit reads with qualities lower than the specified value. Reads which have no qualities are not omitted. Default value is 0.
* _\--sam_ Output aligned reads in SAM format. Default value is false.

For example:

Build index for the reference sequence:
```shell
ugene --genome-aligner --build-index --reference=/path/to/ref
```

Align short reads using the existing index:
```shell
ugene --genome-aligner --reference=/path/to/ref --short-reads=/path/to/reads --result=/path/to/result