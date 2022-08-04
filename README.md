# rmacc22-dask-hpc
Tutorial materials from the Dask on HPC session at the RMACC 2022 Symposium

## Setting up Python to run Dask

The miniconda package environment manager makes it very easy to deploy Dask anywhere.

1. If conda is not available on your system, first install it:
```
# For example - on x86 Linux platforms
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
# Now start a new shell to finish conda integration into your environment
```
2. Use conda (or mamba) to create a new Python environment with required and [useful] packages:
```
conda create -n my-dask-env -c conda-forge dask dask-jobqueue [matplotlib python-graphviz jupyterlab ipywidgets dask-labextension globus-cli]
```
3. Activate the environment and run python, ipython, or use in Jupyter as a language kernel

## Downloading the dataset

If you wish to follow along during or after the tutorial session, you will need to download the data we use in the following commands. I have made these data available via a Globus endpoint, which you can access at https://www.globus.org. Search for the collection called `RMACC 2022 - HPC Dask Tutorial` and download the data to the main directory of the GitHub repo (the one containing this notebook).
