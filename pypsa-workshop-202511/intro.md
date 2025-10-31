# Welcome to the workshop!
*24-25 November 2025, Gothenburg, Sweden*

This repository contains PyPSA(-Eur) materials for a workshop organized for a broad audience of researchers and industry stakeholders interested in energy system modelling.

The workshop is hosted by **RISE (The research institute of Sweden)** (Dr. Markus Millinger).
The workshop is co-organised by the **ENSYS research group at TU Berlin** — Fabian Neumann and Iegor Riepin — with support from the **RESILIENT project**.

The TU Berlin team gratefully acknowledges funding by the German Federal Ministry for Economic Affairs and Energy (BMWE) under Grant No. 03EI4083A (RESILIENT project) jointly with the CETPartnership (https://cetpartnership.eu/) through the Joint Call 2022, which supports our modelling workshops and public training events.

More about our work in RESILIENT project: [https://resilient-project.github.io/](https://resilient-project.github.io/)

## Google Colab

You can work with the workshop materials without a local Python installation using online service [Google Colab](https://colab.google) which provides an online Python environment. This requires only a Google account.

Open any jupyter notebook and click on the rocket 🚀 in the top right corner. It will launch a Colab workspace in your browser with the jupyter notebook loaded.

If that does not work download the `.ipynb` file and import it in [Google Colab](https://colab.research.google.com/)


## A special note for Windows users

For **Windows users**, note that many company laptops have restrictions for installing new software. In previous workshops, we have found that installations on Windows are more prone to errors so we strongly recommend using Windows Subsystem for Linux (WSL). [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install) or an [Ubuntu Virtual Machine](https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview) are two nice options for using Linux on a Windows machine.

## Setting up your Python environment locally

Python coupled with a package manager provides a way to make isolated, reproducible _environments_ where you have control over all installed packages and configurations. We recommend using [`conda`](https://docs.anaconda.com/miniconda/) to manage your Python environments.

### Install Miniconda

Install the lightweight [`miniconda`](https://docs.conda.io/en/latest/miniconda.html) distribution. You likely don't need the full Anaconda Python Distribution. Here is [a great short article](https://medium.com/data-science/conda-essential-concepts-and-tricks-e478ed53b5b) that contains all the essential concepts and tips about using `conda`.

### Clone the repository

Clone this repository to get the workshop materials:

```bash
git clone https://github.com/resilient-project/pypsa-workshop-202511.git
cd pypsa-workshop-202511
```

### Create and activate the environment

We recommend using the locked environment files from [PyPSA-Eur](https://github.com/PyPSA/pypsa-eur/tree/master/envs) for reproducibility. Download the appropriate file for your platform:

- **Linux (Intel/AMD)**: `linux-64.lock.yaml`
- **macOS (Intel)**: `osx-64.lock.yaml`
- **macOS (Apple Silicon)**: `osx-arm64.lock.yaml`
- **Windows**: `win-64.lock.yaml`

Create the conda environment:

```bash
conda env create -f linux-64.lock.yaml  # replace with your platform's file
conda activate pypsa-eur
```

For detailed installation instructions, including solver setup and platform-specific guidance, see the [PyPSA-Eur installation documentation](https://pypsa-eur.readthedocs.io/en/latest/installation.html)
