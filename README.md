# Predict-and-Save

This software create instances dataset in COCO format (json file) as well as YOLO format (txt files). The purpose of this software is to allow the users to create a dataset without having to label images manually by using a pretrained network.

## Requirements
Python 3.4, Tensorflow 1.3, Keras 2.0.8, numpy, scipy, Pillow, cython, matplotlib, scikit-image, opencv-python, h5py, imgaugand IPython

## Usage
In file predict-n-save.ipynb set the path to the images that will be used as a dataset.

## Predicting your own classes
Modify categories.json with your own classes. In coco.py that is located in config folder, set the value of NUM_CLASSES with the number of your classes in categories.json.
