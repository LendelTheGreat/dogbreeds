# dogbreeds

Simple repository containg exploratory models for the kaggle dogbreeds competition

https://www.kaggle.com/c/dog-breed-identification

## My setup
All is done in python, using keras on tensorflow backend.
As my laptop GPU was gathering dust lately, I decided to run all training on it.
It should easily work on newer GPUs on GCP or AWS as well.
 - Win10
 - python 3.5
 - keras, tensorflow, imgaug (for image augmentations)
 - nvidia drivers and cuda toolkit is requiered for GPU support

## Structure
Raw images should be downloaded from kaggle.

Train images are expected to be in data/train folder.

Test images are expected to be in data/test folder.

Submissions will be created into the submissions/ folder.

All notebooks go into the models/ folder.

## Models
Notebooks that start with 'bottleneck_extract' preprocess the images using pretrained imagenet models and pickle the extracted features.
Notebooks that start with 'bottleneck_NN' are fully connected NNs that do the dogbreeds classification on the bottleneck features, not raw images.


