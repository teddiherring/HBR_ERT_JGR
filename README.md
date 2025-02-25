**[contents](#Contents) | [setup](#Setup) | [running the notebooks](#running-the-notebooks) | [issues](#issues)**

# HBR_ERT
Electrical resistivity tomography data and processing code for the Hudson Bay Railway.

## Contents

This repository has a few things in it so far:


1. [raw data files](./raw%20data): This folder contains raw data, including ERT measurements, topography, and frost table depths. 
2. [formatted data files](./formatted%20data): This folder contains ERT datasets that have been converted to the [BERT unified data format](http://resistivity.net/bert/data_format.html).
3. [inverted results](./inverted%20results): This folder contains images of ERT models.
4. [notebook for data processing](./scripts/inversion/invert_all_HBR_data.ipynb): In this notebook, you can load and invert ERT datasets.
 
## Setup

Here are step-by-step instructions for running these notebooks locally on your machine:

Install Python. You can use [anaconda](https://www.anaconda.com/download/) for this.

Clone this repository by running the following in your command line:

```
git clone https://github.com/teddiherring/HBR_ERT
```

Next, `cd` into the directory you just created:

```
cd HBR_ERT
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
