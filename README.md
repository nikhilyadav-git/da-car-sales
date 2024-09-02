# environment setup
* install dependencies
```console
conda create --prefix ./env pandas numpy matplotlib jupyter
```

* list/activate/deactivate enev
```console
conda env list
conda activate ./env
conda deactivate
```
* notebook extensions
```console
conda install -c conda-forge jupyter_contrib_nbextensions
conda install -c conda-forge jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
jupyter nbextensions_configurator enable --user
```
* launch notebook
```console
jupyter notebook
```

### dependencies
* enev dependencies
```console
conda env export --prefix ./env > environment.yaml
```

### clone enev
```console
conda env create --file environment.yaml --name venv
conda activate venv
```

### pyspark
```console
# create env
conda create -n pyspark-env
# activate env
conda activate pyspark-env
# install pyspark package
conda install pyspark
# jupyter kernels
jupyter kernelspec list
# install pyspark kernel
conda install ipykernel
python -m ipykernel install --user --name=pyspark-env
# find spark package
conda install -c conda-forge findspark
# open notebook and select 'pyspark-env' kernel
jupyter notebook
```