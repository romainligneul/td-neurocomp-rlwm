# Neurocomp Pratical - RLWM task modeling

The initial paper by Collins et al. describing the RLWM model (and task) is available in the resources folder.

In this practical, we will:
- simulate variants of the RLWM model
- simulate variants and recovery them by fitting simulated data (as well as their parameters)
- fit real task data (possibly)

> [!IMPORTANT]  
> Please follow the steps below ("Preparing the practical session") to prepare the practical session, and avoid needing internet during the session itself.

> [!NOTE]  
> The notebook A_import_csv_data.ipynb won't run as it needs the raw data, but only the imported/preprocessed_data is available for this tutorial. It is here just for reference

## Preparing the practical session

### 1 - Getting VScode or equivalent (IDE)

Install [VScode](https://code.visualstudio.com/) and download the [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) and [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extensions.

### 2 - Cloning properly this repository

You will need a [Github](https://github.com/) account, [Git](https://git-scm.com/) and the [Github CLI](https://cli.github.com/)

Then, open a terminal (in VScode or anywhere else), navigate to the folder in which you want to have the repository and type:
`git clone https://github.com/romainligneul/td-neurocomp-rlwm`

You may feel tempted to just download the zip archive of the repo. That's a bad idea :)

### 3 - Creating a Python environment

We need to work with specific Python packages using notebooks inside VScode. To do so, you'll need the following dependencies installed:
ipykernel, jupyter, pandas, numpy, matplotlib, pingouin, seaborn, statsmodels, pybads

In order to avoid interfering with your other Python projects you can use [uv](https://docs.astral.sh/uv/). If you are more familiar with other methods, that's fine too. 

This repository comes with a uv.lock file. To create the environment, just type `uv sync` in the terminal (being in this repository)

You might need to register the Python kernel for VScode to detect it. To do so, copy past this line:
```{bash}
uv run python -m ipykernel install --user --name python311 --display-name "Python 3.11 (uv)"
```
