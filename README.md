
# Detecting temporal and spatial malaria patterns from first antenatal care visits

This repository contains the code used to generate the results of the analysis
of the manuscript 'Detecting temporal and spatial malaria patterns from first
antenatal care visits', and some simulated data to validate the performance of
the codes.

Software requirements:
----------------------
The software has been tested using Python 3.8 in a Linux Ubuntu 20.04.4 LTS,
OS type 64-bit and GNOME version 3.36.8.

All the packages that are required are:
- pyhon 3.8
- numpy
- scipy version 1.7 or newer
- pandas
- geopandas version 0.9 or newer
- openpyxl
- jupyter lab
- matplotlib
- contextily

And the following local packages:
- EpiFRIenDs version 1.0
- stat_tools
- pregmal_pytools
- spatial_tools
- genomic_tools

Installation instructions:
--------------------------
The installation of the packages was done using conda. For instruction to
install conda in you computed, we refer to the
[conda website](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).

For the whole installation procedure, open a Unix terminal to run all the
commands described below.
First, we recommend creating a virtual environment with Python3.8
for this specific analysis:
`conda create -n py38 python=3.8 anaconda`
And then activate the environment:
`conda activate py38`

Once activated, install the required packages:
`conda install ipython jupyter jupyterlab numpy pandas geopandas matplotlib scipy`

`conda install -c conda-forge contextily`

`conda install -c anaconda openpyxl`

Then, install the local packages EpiFRIenDs v1.0, stat_tools, pregmal_pytools,
spatial_tools and genomic_tools.

For this, go to each of their directories, and once there, run:

`python setup.py install`

All the packages should be correctly installed. The whole process should not
take more than one hour, unless the full anaconda package is installed instead
of miniconda (see [conda website](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)).

How to use the demos:
----------------------------

To test the performance of the scripts, go to the `demos` directory and lunch
Jupyter lab, for example by running `jupyter lab` in a Unix terminal.

All the Jupyter notebooks should run correctly. As they are by default, they
show the expected output of each cell run and the computational time taken for
the longest runs of the scripts. Most of the notebooks take a few minutes to
run, only one or two can take more than one hour in a normal desktop computer.
Notice that the demos use a simulated data that does not reproduce the results
of the manuscript, but this data is in the exact format used in the manuscript
to properly test the performance of the software.
