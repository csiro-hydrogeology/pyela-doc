# 'ela' (pyela) documentation

This repository hosts documentation for the [Python package 'ela'](https://github.com/jmp75/pyela) (Exploratory Lithology Analysis)

[![Getting started tutorial - Bungendore 3D lithology](https://raw.githubusercontent.com/csiro-hydrogeology/pyela-doc/master/tutorials/img/3d_overlay_bungendore_clay_lithology_small.png "Getting started tutorial - Bungendore 3D lithology")](https://github.com/csiro-hydrogeology/pyela-doc/blob/master/tutorials/getting_started.ipynb)

## Tutorials

NBViewer will render the following notebooks correctly if you want to browse tutorials without installing.

* [Getting Started](https://nbviewer.jupyter.org/github/csiro-hydrogeology/pyela-doc/blob/master/tutorials/getting_started.ipynb)
* [Lithology classification - methods comparisons](https://nbviewer.jupyter.org/github/csiro-hydrogeology/pyela-doc/blob/master/tutorials/lithology_classification_ml.ipynb)

To run the tutorials on your machine, we **strongly** recommend you use conda, e.g. [miniconda](https://docs.conda.io/en/latest/miniconda.html) for Python 3. The following instructions should set things up for running.

### Linux 

```bash
cd $HOME/src
git clone git@github.com:csiro-hydrogeology/pyela-doc.git
```

if for some reasons you do not wish to clone:

```bash
wget https://raw.githubusercontent.com/https://github.com/csiro-hydrogeology/pyela-doc/blob/master/tutorials/getting_started.ipynb
```

```bash
wget https://raw.githubusercontent.com/csiro-hydrogeology/pyela-doc/master/configs/ela_doc_environment.yml
my_env_name=ela_doc
conda env create -n $my_env_name -f ./ela_doc_environment.yml python=3.7
conda activate $my_env_name 
python -m ipykernel install --user --name ${my_env_name} --display-name "Py3 $my_env_name"
```

#### Optional

To activate the possible interactive widgets in notebooks we need `nodejs` installed. If not already on your system, you may use a conda package:

```bash
conda install -n $my_env_name nodejs
```

Then the following should register the `widgets`

```bash
jupyter-labextension install @jupyter-widgets/jupyterlab-manager
```

```bash
cd $HOME/src/pyela-doc
jupyter-lab .
```

### Windows

```bat
cd %USERPROFILE%\src
git clone git@github.com:csiro-hydrogeology/pyela-doc.git
```

or download [getting_started.ipynb](https://raw.githubusercontent.com/csiro-hydrogeology/pyela-doc/master/tutorials/getting_started.ipynb)

Download [ela_doc_environment.yml](https://raw.githubusercontent.com/csiro-hydrogeology/pyela-doc/master/configs/ela_doc_environment.yml)

```bat
set my_env_name=ela_doc
conda env create -n %my_env_name% -f ./ela_doc_environment.yml python=3.7
conda activate %my_env_name% 
python -m ipykernel install --user --name ${my_env_name} --display-name "Py3 %my_env_name%"
```

#### Optional

To activate the possible interactive widgets in notebooks we need `nodejs` installed. If not already on your system, you may use a conda package:

```bash
conda install -n $my_env_name nodejs
```

Then the following should register the `widgets`

```bash
jupyter-labextension install @jupyter-widgets/jupyterlab-manager
```

```bat
cd %USERPROFILE%\src\pyela-doc
jupyter-lab .
```

## Copyrights and License

This source code is under an MIT-like license (see [License.txt](https://github.com/jmp75/pyela/blob/master/LICENSE.txt))

Sample input data used by this notebook can be used for learning purposes. Data from the australian National Groundwater Information System is covered by a [Creative Commons license](http://www.bom.gov.au/water/groundwater/ngis/copyright.shtml). The digital elevation model is extracted from the [SRTM-derived 1 Second Digital Elevation Models Version 1.0](https://ecat.ga.gov.au/geonetwork/srv/eng/catalog.search#/metadata/72759) (Creative Commons Attribution 4.0 International Licence)

