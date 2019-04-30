# segyio-notebooks #

Interactive notebooks with examples and tutorials using the
[segyio](https://github.com/equinor/segyio) library for reading, manipulating 
and writing SEG-Y files.


## Index ##

* [Overview](#Overview)
* [Tutorials](#Tutorials)
* [Data](data)

## Overview ##
In order to ensure that everyone can run the notebooks and produce the expected results, 
each notebook (or set of notebooks sharing a common Python environment) has to be placed in a subdirectory within the
``notebooks`` directory alongside with a ``requirements.txt`` and/or ``environment.yml`` file to be used to create the same
virtualenv and/or condaenv used by the author of the notebook.


## Tutorials ##
Tutorials are organized in subfolders of the ``notebooks`` directory as follows:

**Basic**

- [01 - Basic tutorial](notebooks/basic/01_basic_tutorial.ipynb) - demonstrate how to read
  two F3 seismic volumes as `NumPy` arrays; manipulate the similarity to create
  a discontinuity/fault volume; create a fault mask and display a couple of
  amplitude time slices with superimposed faults; write the fault volume to
  SEG-Y file using re-using the headers from the input file.

**PyLops**

- [01 - Seismic inversion with segyio and pylops](notebooks/pylops/01_seismic_inversion.ipynb) - demonstrate how to download and 
  read a SEG-Y file, perform colored inversion to a portion of the data and saved the inversion result in a brand new SEG-Y.


## Data ##
Data are organized in subfolders of the ``data`` directory. Subfolders should have the same name of the corresponding folders in the 
``notebooks`` tree. Note that some files may exceed the size allowed by github. In that case it is **required** to provide a set of 
instructions in the notebook on how to download the file and it will be assumed that the file will be placed by the user
in the correct subdirectory of ``data``.

**Basic**

Two seismic volumes in SEGY format from the [F3 dataset, offshore
Netherlands](https://terranubis.com/datainfo/Netherlands-Offshore-F3-Block-Complete),
licensed CC-BY-SA: a similarity volume, and an amplitude volume (with dip
steered median filter smoothing applied)

**PyLops**

The seismic cube used in this example is too big to be included in this repo. A set of commands to download the file and place it in the ``data`` 
directory is provided within the notebook.


#### Run the notebooks interactively in Binder
To open and run notebooks interactively in an executable environment, just
click the button below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/equinor/segyio-notebooks/master)
