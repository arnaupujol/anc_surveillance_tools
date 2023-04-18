
# Detecting temporal and spatial malaria patterns from first antenatal care visits

This repository contains the code used to generate the results of the analysis
of the manuscript Pujol et al., 'Detecting temporal and spatial malaria patterns from first
antenatal care visits', Nature Communications 2023.

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
- [EpiFRIenDs version 1.0](https://github.com/arnaupujol/epifriends)
- [stat_tools version 1.0](https://github.com/arnaupujol/stat_tools)
- [pregmal_pytools version 1.0](https://github.com/arnaupujol/pregmal_pytools)
- [spatial_tools version 1.0](https://github.com/arnaupujol/spatial_tools)
- [genomics version 1.0](https://github.com/arnaupujol/genomics)

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
`conda install ipython jupyter jupyterlab numpy pandas geopandas>=0.9 matplotlib scipy>=1.7`

`conda install -c conda-forge contextily`

`conda install -c anaconda openpyxl`

Then, install the packages from the repositories [EpiFRIenDs v1.0](https://github.com/arnaupujol/epifriends), [stat_tools 1.0](https://github.com/arnaupujol/stat_tools), 
[pregmal_pytools 1.0](https://github.com/arnaupujol/pregmal_pytools), [spatial_tools 1.0](https://github.com/arnaupujol/spatial_tools) and [genomics 1.0](https://github.com/arnaupujol/genomics).

For this, clone the repositories or download and uncompress the zip file of the release, 
and once there, run:

`python setup.py install`

All the packages should be correctly installed. The whole process should not
take more than one hour, unless the full anaconda package is installed instead
of miniconda (see [conda website](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)).

How to use the demos:
----------------------------

To test the performance of the scripts, go to the `demos` directory and lunch
Jupyter lab, for example by running `jupyter lab` in a Unix terminal. A data 
directory would be required containing the databases required for the analyses. 
The original data of Pujol et al. 'Detecting temporal and spatial malaria patterns 
from first antenatal care visits', Nature Communications 2023 can be requested 
by email to alfredo.mayor@isglobal.org. 

All the Jupyter notebooks should run correctly. As they are by default, they
show the expected output of each cell run and the computational time taken for
the longest runs of the scripts. Most of the notebooks take a few minutes to
run, only one or two can take more than one hour in a normal desktop computer.

