# Python and PyGOM tutorial


## Abstract
Python is one of the most commonly used coding languages, hosting an extensive array of packages in Data Science, Mathematics
and Machine Learning. With a syntax that emphasis readability, Python is considered one of the easiest coding languages 
to learn. It is also free and open source. Therefore, Python code produced in a research project can be more easily shared
with others and is more accessible outside of academic institutions. In this class, we will begin by introducing Jupyter Notebook (the medium in which this practical will be given) and the basics of python.
We will then introduce several useful python packages, starting with Numpy and Matplotlib. Numpy provides support for handling
multidimensional arrays and matrices. Matplotlib provdes features for producing publishable graphics. The final mandatory section of this class with introduce PyGOM. PyGOM provides a toolbox for modeling with Ordinary Differential Equations (ODEs). Having been developed by the UK Health Security Agency, PyGOM has an emphasis on epidemiological modelling. Providing functionality not only for solving ODEs, parameter estimation and stochastic simulation, but methods for deriving the basic reproduction number R<sub>0</sub>. There is also an optional section covering other useful python packages.

## Instructions


This 2 part tutorial was given on 9<sup>th</sup> and 16<sup>th</sup> January 2024. It irs given in 2 Jupyter Notebooks "Basics_of_Python.ipnyb" (Part 1) and "Python_and_PyGOM.ipnyb" (part 2). With only having one afternoon 16<sup>th</sup> July 2026 we may not get to "Python_and_PyGOM.ipnyb" (part 2). These is some bonus material on the use of Sympy in "R0 in Sympy and PyGOM".  Before using the notebook you will need to follow the installation instructions below.
To use the notebook open Anaconda prompt use the command:
* `conda activate pygom`
* `cd *directory housing ""*` to navigate to the diretory housing "Python_and_PyGOM.ipnyb"
* `jupyter notebook` This should open a web browser window. Double click "Python_and_PyGOM.ipnyb" to open it and begin tutorial.

## Download this repository
To download this specific repository you need to first install git (see section 2.1). Then open git bash (or terminal) and enter the following commands:
1. `cd *download location*` replace \*download location\* with the name of the folder you wish to download this repository to.
2. `git clone https://github.com/m-d-grunnill/Python-and-PyGOM-tutorial.git`

To update this repository in git bash:
1. `cd *repository*` replace \*repository\* with the location of this repository.
2. `git pull`


## Installation Instructions

### 1. Prerequisites: C++ Compiler

PyGOM relies on Cython which uses C++ to speed up runtime. You will need a C++ compiler installed **before** creating the conda environment. This differs by OS:

#### Windows: Installing Microsoft C++ Build Tools
1. Go to this link and download Microsoft C++ Build Tools: https://visualstudio.microsoft.com/visual-cpp-build-tools/.
2. Download Microsoft C++ Build Tools:

![image info](./readme_images/Download%20Microsoft%20C++%20Build%20Tools.png)
3. Once downloaded open vs_BuildTools.exe and navigate too "Available":

![image info](./readme_images/Available.png)
4. Select installation of community edition:

![image info](./readme_images/community_edition.png)

5. Select "Desktop development with C++":

![image info](./readme_images/Desktop_development.png)
6. Optional: To save on memory you can deselect everything but "MSVC v143 – VS 2022 C++ x64/x86 build tools (Latest)" and "Windows [your version of Windows] SDK":

![image info](./readme_images/memory_save.png)
7. Then click install:

![image info](./readme_images/install_build_tools.png)

8. Once installed Visual Studio may start simply close it.
9. Restart your computer.

#### Mac: Installing Xcode
Follow the instructions outlined in either:
* [https://support.wolfram.com/12799?src=system-modeler](https://support.wolfram.com/12799?src=system-modeler)
* The first 1 min and 48 seconds of [https://www.youtube.com/watch?v=ENy4MdoOxug](https://www.youtube.com/watch?v=ENy4MdoOxug)

#### Linux: Installing GCC
Follow Steps 1-2 from [https://www.cyberciti.biz/faq/howto-compile-and-run-c-cplusplus-code-in-linux/](https://www.cyberciti.biz/faq/howto-compile-and-run-c-cplusplus-code-in-linux/)

### 2. Creating the Conda Environment

Once you have a C++ compiler installed, create the conda environment using the provided `conda-env.yml` file. This will install Python, PyGOM, and all other required packages.

1. Install [Anaconda](https://docs.anaconda.com/free/anaconda/install/index.html) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
2. Open Anaconda prompt (or terminal) and navigate to this repository:
   ```
   cd /path/to/Python-and-PyGOM-tutorial
   ```
3. Create the environment:
   ```
   conda env create -f conda-env.yml
   ```
   Or if you have mamba installed:
   ```
   mamba env create -f conda-env.yml
   ```
4. Activate the environment:
   ```
   conda activate pygom
   ```
5. Verify PyGOM is installed:
   ```
   python -c "import pygom; print(pygom.__version__)"
   ```
