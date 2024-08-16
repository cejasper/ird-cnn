# EXP382

# Requirements

## CUDA

You need to be running CUDA 10.0 (10.1 might work now) to use tf2.

## Environment files

The environment file (EXP382.yml) contains the package requirements needed to run the notebooks in this repository. Create a local anaconda environment on your machine from the .yml file:

> conda env create -f EXP382.yml

if the .yml file has changed, sync your env to the new file with:

> conda env update --name EXP382 --file EXP382.yml

activate that environment:

> conda activate EXP382

 and run jupyter:

> jupyter notebook

or

> jupyter lab
