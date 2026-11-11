
# Climate Date Rescue Utilities

This library wraps a set of functions used for climate data rescue
projects in a modern python package. Thie facilitates version
history and ease of importing these functions instead of copying the same
code in multiple projects.

The python implementation of {lmrlib} is take fropm 
(https://github.com/chesleymccoll/CS3-DR-Unit_Conversions) and wrapped in
Python class {lmrlib}.

The ISO mappings come from the DRAW project and are wreapped in the Python
class {iso_mapping}

## Using the utilites

We recommend that you use {uv} for you python project. You can then add
the dependancy to these utilities via the command

```
uv add cdr-utilities
```

and within your python code import the functionality via

```
from cdr-utilities import iso_mapping
from cdr-utilities import lmrlib
```

Access the functions via

```
# Barometer mm to mb - using 9mm
lmrlib.baro_mm2mb(760.)
```

## Development notes

Ensure that you have the following utilities installed

```
uv
twine
```

Initialize the project with

```
uv synv
```

and build locally with

```
uv build
```

You can check the build package with

```
twine check dist/*
```
