# nxt_graphs_usd

![Alt text](images/stageopen.PNG?raw=true "StageOpen")

## Overview

A library of USD graphs/nodes for use inside NXT with some simple USD examples. 

## Important Links

 - Please insure that you have both [NXT](https://nxt-dev.github.io/) and [USD](https://github.com/PixarAnimationStudios/USD) setup on your pc.
 - How to use the USD library nodes: [Example](Example.md) 

## Coding guidelines for Python

We are adopting the [PEP-8](https://www.python.org/dev/peps/pep-0008) style for Python Code with the following modification:
* Mixed-case for variable and function names are allowed 

____________________________________

Supported Platforms
-------------------

These graphs have been tested on Centos 7.7

Dependencies
------------

The following dependencies are required:

 - [Python](https://python.org)
 - Please see NXT and USDs documentation for their dependencies.

**usdview**

 - [PySide](http://wiki.qt.io/PySide) or [PySide2](http://wiki.qt.io/PySide2)
 - [PyOpenGL](https://pypi.python.org/pypi/PyOpenGL/)

### Setup up NXT env with USD

Making a nxt.sh:
```
#!/usr/bin/bash

# PATH TO USD
export PYTHONPATH="$PYTHONPATH:PATH/TO/USD/lib/python"
export PATH="$PATH:PATH/TO/USD/bin"
export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:PATH/TO/USD/lib"
# NXT ROOTS
export NXT_FILE_ROOTS="/path/too/work/space"
# Run NXT
nxt ui
```

This can now be run in terminal: ``` ./nxt.sh ```

