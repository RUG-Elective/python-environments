# Using mamba to create the Geospatial environment

## Starting steps
This briefly describes how to install a Python virtual environment for the Geo-Python course.

1. Install miniconda from https://docs.conda.io/en/latest/miniconda.html
2. Install mamba
    ```bash
    conda install mamba -n base -c conda-forge
    ```
3. Clone the course Python environments from GitHub
    ```bash
    git clone https://github.com/RUG-Elective/python-environments.git
    ```
4. Change into the working directory with the cloned environment files
    ```bash
    cd python-environments
    ```
## Creating the environment for students
1. Create the python environment using mamba
    ```bash
    mamba env create -f geospatial-student.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    conda activate geospatial-student
    sh postBuild
    ```
