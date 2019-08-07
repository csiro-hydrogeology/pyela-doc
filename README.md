# 'ela' (pyela) documentation

This repository hosts documentation for the [Python package 'ela'](https://github.com/jmp75/pyela) (Exploratory Lithology Analysis)

## Installation 

The quickest way with conda:

```bash
wget https://raw.githubusercontent.com/csiro-hydrogeology/pyela-doc/master/configs/ela_doc_environment.yml
my_env_name=eladoc
conda env create -n $my_env_name -f ./ela_doc_environment.yml python=3.7
conda activate $my_env_name 
jupyter-labextension install @jupyter-widgets/jupyterlab-manager
python -m ipykernel install --user --name ${my_env_name} --display-name "Py3 $my_env_name"
```

## Tutorials

* [Getting Started](./tutorials/getting_started.ipynb)
* [Lithology classification - methods comparisons](./tutorials/lithology_classification_ml.ipynb)

## License

* The source code is under an MIT-like license (see [License.txt](https://github.com/jmp75/pyela/blob/master/LICENSE.txt))
* Sample input data may be linked to and licensed at a later date.

