# Predict-and-Save

## Introduction
Object detection is an AI that requires training with huge amount of dataset. Preparing the dataset is a trivial process as it has to be done manually. A lot of images has to be labelled manually using different tools such as [Coco-Annotator](https://github.com/jsbroks/coco-annotator.git) and [labelImg](https://github.com/tzutalin/labelImg). Predict-and-Save helps the user to label new images using a pretrained model. This will reduce the workload of the users who want to prepare their own dataset.

## Output
predict-n-save.ipynb will generate dataset with 2 different formats, as different labeling tools use different dataset format.
1. **COCO Json format**  
Prediction will be stored in Json file with [COCO format](https://www.immersivelimit.com/tutorials/create-coco-annotations-from-scratch). With tools such as [Coco-Annotator](https://github.com/jsbroks/coco-annotator.git) the user can import the json file and modify the annotations.
2. **txt files with YOLO format**  
Annotations are also saved in [YOLO format](https://github.com/AlexeyAB/Yolo_mark/issues/60). One common tools that uses this format to label images is [labelImg](https://github.com/tzutalin/labelImg).

## Requirements
Python 3.4, Tensorflow 1.3, Keras 2.0.8, numpy, scipy, Pillow, cython, matplotlib, scikit-image, opencv-python, h5py, imgaug and IPython

## Predicting your own classes
Modify categories.json with your own classes. In coco.py which is located in config folder, set the value of NUM_CLASSES with the number of your classes in categories.json.
