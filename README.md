# Python Tutorial


## Abstract
Python is one of the most commonly used coding languages, hosting an extensive array of packages in Data Science, Mathematics
and Machine Learning. With a syntax that emphasises readability, Python is considered one of the easiest coding languages
to learn. It is also free and open source. Therefore, Python code produced in a research project can be more easily shared
with others and is more accessible outside of academic institutions. In this class, we will begin by introducing Jupyter Notebook (the medium in which this practical will be given) and the basics of Python.
We will then introduce several useful Python packages, starting with Numpy and Matplotlib. Numpy provides support for handling
multidimensional arrays and matrices. Matplotlib provides features for producing publishable graphics. We also cover Pandas for data manipulation, Seaborn for statistical visualisation, and Sympy for symbolic mathematics.

## Instructions

This tutorial is given in 2 Jupyter Notebooks:
- `Basics_of_Python.ipynb` (Part 1)
- `Python_packages_for_Applied_Maths.ipynb` (Part 2)

Before using the notebooks you will need to follow the installation instructions below.
To use the notebooks, open Anaconda prompt and run:
1. `conda activate python_tutorial`
2. `cd /path/to/Python-and-PyGOM-tutorial`
3. `jupyter notebook`

This should open a web browser window. Double click a notebook to open it and begin the tutorial.

## Download this Repository
To download this repository you need to first install git. Then open git bash (or terminal) and enter the following commands:
1. `cd /download/location` — replace with the folder you wish to download this repository to.
2. `git clone https://github.com/m-d-grunnill/Python-and-PyGOM-tutorial.git`

To update this repository:
1. `cd /path/to/Python-and-PyGOM-tutorial`
2. `git pull`


## Installation Instructions

1. Install [Anaconda](https://docs.anaconda.com/free/anaconda/install/index.html) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
2. Open Anaconda prompt (or terminal) and navigate to this repository:
   ```
   cd /path/to/Python-and-PyGOM-tutorial
   ```
3. Create the environment:
   ```
   conda env create -f environment.yml
   ```
   Or if you have mamba installed:
   ```
   mamba env create -f environment.yml
   ```
4. Activate the environment:
   ```
   conda activate python_tutorial
   ```
