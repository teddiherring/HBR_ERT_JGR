**[contents](#Contents) | [setup](#Setup) | [running the notebooks](#running-the-notebooks) | [issues](#issues)**

# HBR_ERT_JGR
Electrical resistivity tomography data and processing code for the Hudson Bay Railway. 

This repository supports a manuscript titled "Relationships Between Permafrost Distribution and Surface Conditions Along the Hudson Bay Railway Evaluated Using Electrical Resistivity Tomography" by Herring et al., submitted to the Journal of Geophysical Research: Solid Earth.

## Contents

This repository has a few things in it so far:


1. [ERT data](./formatted%20ert%20data): This folder contains raw ERT measurements in the [BERT unified data format](http://resistivity.net/bert/data_format.html).
2. [borehole data](./borehole%20data): This folder contains measured borehole temperatures.
3. [frost tables ](./frost%20tables): This folder contains measured frost table depths.
4. [notebook to determine resistivity-temperature relationships](./generate_rho_T_curves.ipynb): This notebook plots co-located ERT and temperature data and determines best-fit curves.
5. [notebook for data processing](./invert_ert_data.ipynb): This notebook inverts the ERT datasets and estimates the boundary between frozen and unfrozen subsurface regions.
 
## Setup

Here are step-by-step instructions for running these notebooks locally on your machine:

Install Python. You can use [anaconda](https://www.anaconda.com/download/) for this.

Clone this repository by running the following in your command line:

```
git clone https://github.com/teddiherring/HBR_ERT_JGR
```

Next, `cd` into the directory you just created:

```
cd HBR_ERT_JGR
```

You can use the provided conda environment to set up the necessary software packages:

```
conda env create -f environment.yml
conda activate hbr
```

Next, running the following command

```
jupyter notebook
```

will open a Jupyter notebook in your web browser. You can now open the data processing notebook and start running the code.

## Running the notebooks

You can run each cell in the notebook individually by pressing  `shift + enter`, or you can run the entire notebook by selecting `Cell`, `Run All` in the toolbar.

## Issues

Please [make an issue](https://github.com/teddiherring/HBR_ERT/issues) if you encounter any problems while trying to run the notebooks.
