## Index ##

* [Data](data)
* [Tutorials](#Tutorials)

## Data ##
Two seismic volumes in SEGY format from the [F3 dataset, offshore Netherlands](https://terranubis.com/datainfo/Netherlands-Offshore-F3-Block-Complete), licensed CC-BY-SA: a similarity volume, and an amplitude volume (with dip steered median filter smoothing applied)

## Tutorials ##
A set of Jupyter notebook tutorials of increasing complexity.

- [01 - Basic tutorial](01_basic_tutorial.ipynb) - demonstrate how to read the two F3 seismic volumes as `NumPy` arrays; manipulate the similarity to create a discontinuity/fault volume; create a fault mask and display a couple of amplitude time slices with superimposed faults; write the fault volume to SEGY file using re-using the headers from the input file.

#### Run the notebooks interactively in Binder
To open and run notebooks interactiely in an executable environment, just clikck the button below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/equinor/segyio-notebooks/master)
