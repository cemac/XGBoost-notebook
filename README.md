<div align="center">
<a href="https://www.cemac.leeds.ac.uk/">
  <img src="https://github.com/cemac/cemac_generic/blob/master/Images/cemac.png"></a>
  <br>
</div>

# Machine Learning for the Earth Sciences

# Gradient Boosting with XGBoost

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cemac/XGBoost-notebook/HEAD?labpath=XGBoost.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cemac/XGBoost-notebook/blob/main/XGBoost.ipynb)

In this tutorial notebook, we will run through the process of fitting [XGBoost](https://xgboost.readthedocs.io/en/stable/) models to meteorological data from the [SHEBA campaign](https://www.eol.ucar.edu/field_projects/sheba), in order to predict surface turbulent fluxes of sensible heat over sea ice in the Arctic. This application to polar turbulent fluxes, inspired by the work of [Cummins et al. (2023)](https://doi.org/10.1029/2023GL105698) and [Cummins et al. (2024)](https://doi.org/10.1007/s10546-023-00852-8), is an example of a parametrization problem that is hard to solve with traditional physics, and illustrates how modern boosting methods allow us to easily obtain performant models.

## Notebook Prerequisites

Readers are assumed to have basic familiarity with the programming language [Python](https://www.python.org/), and to have already completed the [tutorial notebook on Random Forests](https://github.com/cemac/LIFD_RandomForests) from the [Leeds Institute for Fluid Dynamics (LIFD)](https://fluids.leeds.ac.uk/).

## Running Locally

If you're already familiar with Git, [Anaconda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) and virtual environments, the environment you need to create is found in [XGB.yml](XGB.yml) and the code below will install, activate and launch the notebook. The .yml file has been tested on the Windows 11 operating system.

```bash
git clone git@github.com:cemac/XGB-notebook.git
cd XGB-notebook
conda env create -f XGB.yml
conda activate XGB
jupyter-notebook
```

# Licence information #

![licence](https://i.creativecommons.org/l/by/4.0/88x31.png)

XGBoost-notebook by [CEMAC](https://www.cemac.leeds.ac.uk/) is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
