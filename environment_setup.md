# Environment Set Up for Data Analysis in Python

### How to set up pytorch with Nvidia GPU support

- Download and install the CUDA toolkit version from the Nvidia website that is compatible with your system's 
  current Nvidia GPU 
  (which can also be checked on the Nvidia website).
- Create a new conda environment `conda create --name cpsc445 python=3.9` with python 3.9 since this is the latest 
  python version that works with pytorch (as of April 1, 2023)
- Activate your new environment `conda activate cpsc445` (where cpsc445 is the environment name)
- Run `conda install pytorch cudatoolkit=11.7`, replacing the cudatoolkit argument with the version of the toolkit 
  you downloaded from the Nvidia website.
- Verify your GPU is available to use with pytorch by running the following in python:
```python
import torch
print(torch.cuda.is_available())
```

### Download Packages
Activate conda environment and run
- `conda install -c conda-forge scanpy python-igraph leidenalg`
- `conda install -c conda-forge imbalanced-learn`
- `conda install -c conda-forge xgboost`
- `conda install -c conda-forge lightgbm`
- `conda install -c conda-forge catboost`


altogether??
`conda create -p \home\ptellier\scratch\phillip\my_jupyter\445proj python=3.9`
`conda install -c conda-forge scanpy python-igraph leidenalg imbalanced-learn xgboost lightgbm catboost`
