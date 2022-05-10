# Cookiecutter ML

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._

Insipred by [cookiecutter-data-science-poetry-makefile](https://github.com/IngerMathilde/cookiecutter-data-science-poetry-makefile) and [cookiecutter-data-science](http://drivendata.github.io/cookiecutter-data-science/)


### How to use the cookiecutter template:
-----------
 - Install conda/mamba 
 - Use env.yml file to create an environment (change env name in the file)

``` bash
conda env create -f env.yml
```
 - Activate newly create environment:
 
``` bash
conda activate ml
```

- To start a new project, run:
``` bash
cookiecutter https://github.com/paulvstrashnov/cookiecutter_ml
```

### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── 01_raw         <- The original, immutable data dump.
│   ├── 02_interim     <- Intermediate data that has been transformed.
│   ├── 03_processed   <- The final, canonical data sets for modeling.
│
├── models             <- Trained and serialized models, model predictions, or model summaries.
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│
├── pyproject.toml     <- The file for reproducing the environment using [Poetry](https://python-poetry.org/)
│
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes {{ cookiecutter.source_name }} a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── __init__.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── __init__.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── __init__.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── __init__.py
│
├── Dockerfile
├── docker-compose.yml
├── docker-compose.yml
├── .pre-commit-config.yaml  <- Config file for [pre-commit](https://pre-commit.com/)
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io

```
