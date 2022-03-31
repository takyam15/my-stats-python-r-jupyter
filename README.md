# my-stats-python-r-jupyter

Here is my programming environment for basic statistical data analysis and machine learning.
Main features are:
* Interactive data analysis using JupyterLab
* Environment with both Python and R


## Requirements

* conda (if Docker is not used)
* Docker (if used)


## Installation

### Getting started with Docker

Clone this repository and run:

```bash
docker compose build
```

or you can pull the docker image from [my DockerHub repository](https://hub.docker.com/repository/docker/takyam15/my-stats-python-r-jupyter)

After building or downloading docker image run:

```bash
docker compose up -d
```

Then JupyterLab will be loaded by accessing `localhost:8888` on your web browser.

You can check libraries are successfully installed by running `env_checker.ipynb` in `Python` and `R` directories.


### Getting started without Docker

Clone this repository and run:

```bash
conda update conda
conda env create --file base_env.yml
conda activate stats
conda install -y -c conda-forge --file requirements_conda.txt
pip install --upgrade pip
pip install -r requirements_pip.txt
```

With the developed environment activatad, run `jupyter-lab` command, and JupyterLab will be loaded on your web browser.

You can check libraries are successfully installed by running `env_checker.ipynb` in `Python` and `R` directories.


## Note

Python libraries for deep learning are not installed in this environment.
For deep learning another environment should be used.
