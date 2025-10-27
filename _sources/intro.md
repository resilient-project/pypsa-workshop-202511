# Welcome to the workshop!
*24-25 November 2025, Gothenburg, Sweden*

This repository contains PyPSA(-Eur) materials for a workshop organized for a broad audience of researchers and industry stakeholders interested in energy system modelling.

The workshop is hosted by **RISE (The research institute of Sweden)** — Dr. Markus Millinger — with support from the **ENSYS research group at TU Berlin** (Fabian Neumann and Iegor Riepin) and the **RESILIENT project**.

The TU Berlin team gratefully acknowledges funding by the German Federal Ministry for Economic Affairs and Energy (BMWE) under Grant No. 03EI4083A (RESILIENT project) jointly with the CETPartnership (https://cetpartnership.eu/) through the Joint Call 2022, which supports our modelling workshops and public training events.

More about our work:

- RESILIENT project: [https://resilient-project.github.io/](https://resilient-project.github.io/)

## Google Colab

You can work with the workshop materials without a local Python installation using online service [Google Colab](https://colab.google) which provides an online Python environment. This requires only a Google account.

Open any jupyter notebook and click on the rocket 🚀 in the top right corner. It will launch a Colab workspace in your browser with the jupyter notebook loaded.

If that does not work download the `.ipynb` file and import it in [Google Colab](https://colab.research.google.com/)


## Setting up your Python environment locally

### Anaconda

Coordinating the compatibility between different Python software packages and
their multiple versions can be difficult! Fortunately, the problem is solved by
using a Python _distribution_ and/or _package manager_.

For instance, you can install on your computer the popular [Anaconda Python
Distribution](https://www.anaconda.com/download/) or the ligth version `miniconda` described below.

For **Linux and MacOS users**, you can access the command line by opening the
_terminal_ program.

For **Windows users**, note that many company laptops have restrictions for installing new software. In previous workshops, we have found that installations on Windows are more prone to errors so we strongly recommend using Linux. [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install) or an [Ubuntu Virtual Machine](https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview) are two nice options for using Linux on a Windows machine.

## Managing environments with `conda`

Python coupled with a package manager provides a way to make isolated,
reproducible _environments_ where you have control over all installed packages
and configurations. Here is [a great short article](https://medium.com/data-science/conda-essential-concepts-and-tricks-e478ed53b5b) that contains all the essential concepts and tips about using `conda`.

### Tip: use lightweight `miniconda`

Instead of `Anaconda`, you use a lightweight installation called
[`miniconda`](https://docs.conda.io/en/latest/miniconda.html). It is very likely that you don't want the full Anaconda Python Distribution.


## Environment for this course: `workshop`

### ... with `conda` (recommended)

The latest environment specification for this course can be downloaded under the following link as a [`YAML`-file](https://en.wikipedia.org/wiki/YAML):

https://github.com/resilient-project/pypsa-workshop-202511/blob/main/environment.yaml

There is a download button at the top-right corner.

After navigating to the folder where the `environment.yaml` file is stored ([here](https://tutorials.codebar.io/command-line/introduction/tutorial.html)'s a tutorial how to navigate with the command line),
you can reate this environment using `conda`

    conda env create -f environment.yaml

Activate this environment

    conda activate workshop

The environment has to be activated whenever you open a new terminal,
*before* starting a new Jupyter window with

    jupyter lab

### ... with `pip`

If you want to use `pip` for managing your environment, download

https://github.com/resilient-project/pypsa-workshop-202511/blob/main/requirements.txt

There is a download button at the top-right corner.

After navigating to the folder where the `requirements.txt` file is stored,
you can install the required packages with

    pip install -r requirements.txt

This should allow you to start a new Jupyter window:

    jupyter lab
