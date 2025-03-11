# SAR-Doppler-user-guide

User guide for SAR Doppler data - Online version of the user manual is available at: https://metno.github.io/MET_SAR-Doppler_User_Guide/.

To find the ipynb (jupyter notebook) files go to the notebooks folder.

To find the HTML files for the different Jupyter notebooks that collectively
constitute the user guide, go to `_build/html/notebooks and select your desired
notebook`.

The user guide is also available as a PDF. However, with the in place structure of the manual, it is preferable to open it as HTML, indvidual jupyter notebooks or as a jupyter-book. This has to do with certain code snippets and outputs.

Here is the link to the jupyter-book documentation: https://jupyterbook.org/en/stable/intro.html

# Installation

In order to run the examples interactively, install jupyter in a local conda
environment (see
https://docs.conda.io/projects/conda/en/stable/user-guide/install/index.html).
The code below is tested on a linux ubuntu terminal:

```
conda create -n "jupyter" python=3.12
conda activate jupyter
conda install -c conda-forge xarray netCDF4 bottleneck pydap matplotlib cartopy jupyter
pip install fadg@git+https://github.com/metno/esa-coscaw-data-search.git
```

# Run interactive notebooks

In the terminal:

```
conda activate jupyter
jupyter notebook
```

A browser tab should open. Open one of the ipynb files in the file overview.
The code snippets can be run by selecting them, and clicking ctrl-enter.

Note that you can use the web search to find other datasets, and replace
filenames with opendap urls to look at the data you find online.
