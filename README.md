## Multi label image classification - Instruments and Vechicle images

We have a dataset with images possibly belong to multiple classes, therefore we aim to do a multi label image classification model

You can download the images from the dataset at:
https://www.kaggle.com/datasets/meherunnesashraboni/multi-label-image-classification-dataset

To install the project you need to install miniconda locally then you need to do the following actions:

minicoda source: https://docs.anaconda.com/free/miniconda/miniconda-install

1. Create the conda environment - this will create an environment based on what you have in 'environment.yml' file
   command:  conda env create -f environment.yml

2. Activate the environment 
   command: conda activate 'env-name'

3. Optionally you can export your dependencies to an external requirements.txt file
   command: conda list --export > requirements.txt     

4. To update dependencies use the update command and --prune flag to remove all other dependencies that are not longer defined in the .yml file
   command: conda env update -f environment.yml --prune


You can view the training details using tensorboard a package that is installed by default when installing tensorflow. This will open a local server on a specific port and will agregate the logs of the training step. It is mandatory to log the training details using a tensorflow callback.
This can be used by running the following command:
   command: tensorboard --logdir logs


For this project I named my env:  **image-classification-env**  and I used conda to activate it using the following command:
   command: conda activate image-classification-env
   
The images will pe stored as a zip file on github in order to retrain the model extract the archive locally