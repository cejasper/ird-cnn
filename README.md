## Convolutional Neural Network to Identify IRD in IODP Expedition 382 Sediment Cores X-ray Images
Repository for the Jasper et al. (2024) manuscript in Paleoceanography and Paleoclimatology entitled, "A 3.3-Million-Year Record of Antarctic Iceberg Rafted Debris and Ice Sheet Evolution Quantified by Machine Learning"

## This repo has three jupyter notebooks:
#### 1_cnn_build
notebook with the training data set up and the cnn model architecture. 
#### 2_label_images
notebook to use the trained cnn model to label either single images or images down splice 
#### 3_ird_counter
notebook to go from the IRD-labeled images to a csv file with the depth of each IRD grain identified down the splice 

## Additional Information
All of the training data and the trained CNN model used in Jasper et al. (2024) has been archived on Zenodo, and is available for download [here](https://zenodo.org/records/13333689)

Note: The model architecture in 1_cnn_build builds off of the code from Dyer et al. 2021 PNAS and the original model build can be found [here](https://github.com/blakedyer/bahamas_lig)

## Requirements for running and training the CNN model

#### CUDA

You need to be running CUDA 10.0 (10.1 might work now) to use tf2.

#### Environment files

The environment file (tensorflow.yml) contains the package requirements needed to run the notebooks in this repository. Create a local anaconda environment on your machine from the .yml file:
```
conda env create -f tensorflow.yml
```
activate that environment:
```
conda activate tensorflow
```
 and run jupyter:
```
jupyter notebook
```
or
```
jupyter lab
```
