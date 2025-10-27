# Welcome to the workshop!
*24-25 November 2025, Gothenburg, Sweden*

This repository contains PyPSA(-Eur) materials for a workshop organized for a broad audience of researchers and industry stakeholders interested in energy system modelling.

The workshop is hosted by **RISE (The research institute of Sweden)** (Dr. Markus Millinger).
The workshop is co-organised by the **ENSYS research group at TU Berlin** — Fabian Neumann and Iegor Riepin — with support from the **RESILIENT project**. 

TUB team gratefully acknowledges funding by the German Federal Ministry for Economic Affairs and Energy (BMWE) under Grant No. 03EI4083A (RESILIENT project**) jointly with the CETPartnership (https://cetpartnership.eu/) through the Joint Call 2022, which supports our modelling workshops and public training events.

The TU Berlin team gratefully acknowledges funding by the German Federal Ministry for Economic Affairs and Energy (BMWE) under Grant No. 03EI4083A (RESILIENT project) jointly with the CETPartnership (https://cetpartnership.eu/) through the Joint Call 2022, which supports our modelling workshops and public training events.

More about our work in RESILIENT project: [https://resilient-project.github.io/](https://resilient-project.github.io/)

## Google Colab

You can work with the workshop materials without a local Python installation using online service [Google Colab](https://colab.google) which provides an online Python environment. This requires only a Google account.

Open any jupyter notebook and click on the rocket 🚀 in the top right corner. It will launch a Colab workspace in your browser with the jupyter notebook loaded.

If that does not work download the `.ipynb` file and import it in [Google Colab](https://colab.research.google.com/)


## Setting up your Python environment locally

### Using `uv` (recommended)

We recommend using [`uv`](https://docs.astral.sh/uv/) - a fast Python package and project manager. It's significantly faster than traditional tools like `conda` or `pip` and provides excellent dependency resolution.

For **Windows users**, note that many company laptops have restrictions for installing new software. In previous workshops, we have found that installations on Windows are more prone to errors so we strongly recommend using Windows Subsystem for Linux (WSL). [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install) or an [Ubuntu Virtual Machine](https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview) are two nice options for using Linux on a Windows machine.

### Installing `uv`

On **macOS and Linux**:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

On **Windows**:
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

For other installation methods, see the [official uv installation guide](https://docs.astral.sh/uv/getting-started/installation/).

## Setting up the workshop environment

### Clone the repository

First, clone or download this repository:
```bash
git clone https://github.com/resilient-project/pypsa-workshop-202511.git
cd pypsa-workshop-202511
```

### Install dependencies with `uv`

The project dependencies are specified in `pyproject.toml`. To create a virtual environment and install all dependencies:

```bash
uv sync
```

This will:
- Create a virtual environment in `.venv/`
- Install Python 3.13 (if not already available)
- Install all required packages including PyPSA 1.0+
- Create a `uv.lock` file with exact versions

### Activate the environment

**On Linux/MacOS**:
```bash
source .venv/bin/activate
```

**On Windows**:
```powershell
.venv\Scripts\activate
```

### Alternative: Using `pip`

If you prefer using `pip`, you can install from `requirements.txt`:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
```
