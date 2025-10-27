# taskflow - General-purpose Task-parallel Programming System

This is a `build2` package repository for [`taskflow`](https://github.com/taskflow/taskflow),
a general-purpose task-parallel programming system using modern C++.

This file contains setup instructions and other details that are more
appropriate for development rather than consumption. If you want to use
`taskflow` in your `build2`-based project, then instead see the accompanying
[`PACKAGE-README.md`](libtaskflow/PACKAGE-README.md) file.

The development setup for `taskflow` uses the standard `bdep`-based workflow.
For example:

```
git clone https://github.com/build2-packaging/taskflow.git
cd taskflow

bdep init -C @gcc cc config.cxx=g++
bdep update
bdep test
```
