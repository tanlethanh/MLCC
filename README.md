## Setup Python

Prefer using [miniconda](https://docs.anaconda.com/miniconda/) to install, manage Python environments. You need to download `miniconda` [here](https://docs.anaconda.com/miniconda/miniconda-install/)

After correctly setting up `miniconda`, you are able to use it from ternimal

```
# Show version of installed conda
conda --version
```

Create a Python environment for this repository

```
# Create a Python version 3.10 at `.venv` directory from root of this project
conda create --prefix ./.venv python=3.10
```

_Notice that this environment is a virtual environment, might be used, should be used only by this project. This process ensures that there is no packages, libraries messing or conflicting between projects._

To use this virtual environment, you need to activate it

```
# Activate Python venv for current terminal session
conda activate ./.venv
```

_This activation is only available in a terminal session, if you reopen or reload terminal, you will need to reactivate the `venv`_
