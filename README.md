# Predict-and-Save

This software create instances dataset in COCO format (json file) as well as YOLO format (txt files). The purpose of this software is to allow the users to create a dataset without having to label images manually by using a pretrained network. The output from the software (json file and YOLO bouding boxes files) can be modified using another tools such as [coco-Annotator](https://github.com/jsbroks/coco-annotator.git) and [LabelImg](https://github.com/tzutalin/labelImg)

## Requirements
Python 3.4, Tensorflow 1.3, Keras 2.0.8, numpy, scipy, Pillow, cython, matplotlib, scikit-image, opencv-python, h5py, imgaug and IPython

## Output
predict-n-save.ipynb will create a json file that contains the annotations from the prediction. It will also generate files that stored the bounding boxes information in YOLO format.

## Predicting your own classes
Modify categories.json with your own classes. In coco.py that is located in config folder, set the value of NUM_CLASSES with the number of your classes in categories.json.
