# my-stats-python-r-jupyter

Here is my programming environment for statistical data analysis and machine learning.
Both python and R can be executed on JupyterLab.


## Requirements

* conda (if Docker is not used)
* Docker (if used)


## Installation

### Getting started with Docker

Clone this repository and run:

```bash
docker compose build
```

After building docker image run:

```bash
docker compose up -d
```

You can use JupyterLab by accessing `localhost:8888` on your web browser.


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

With the developed environment activatad, run `jupyter-lab` command to start data analysis.


## Note

Python libraries for deep learning are not installed in this environment.
For deep learning another environment should be used.
