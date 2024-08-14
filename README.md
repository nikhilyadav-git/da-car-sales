# environment setup
* install dependencies
```console
conda create --prefix ./env pandas numpy matplotlib jupyter
```
* activate/deactivate enev
```console
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