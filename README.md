# Transfer Learning for Geological Images

## Description
This is the repository for the code in Dawson et al 2022. This code can be used to easily to perform transfer learning for geological images using any of the built-in TensforFlow-Keras image classification models used in the paper.

## Built-In Models
The models available here are:
| Model  | Size  |  Top-1 Accuracy  |  Top-5 Accuracy  |  Parameters  |  Depth  |
| -------------     | ------------- | -------------| ------------- | ------------- | ------------- |
| VGG16    | 528 MB    |  0.713    | 0.901    | 138.4M    | 16    |
| VGG19    | 549 MB    |  0.727    | 0.910    | 143.7M    | 19    |
| ResNet50    |  98 MB    | 0.749    | 0.921    | 25.6M    |  107    |
| ResNet101    |  171 MB    | 0.764    | 0.928    | 44.7M     | 209    |
| ResNet152    |  232 MB    | 0.766    | 0.931    | 60.4M     | 311    |
| InceptionV3    | 92 MB    | 0.779    | 0.937    | 23.9M    |  159    |
| DenseNet121    | 33 MB    | 0.750    | 0.923    | 8.1M    | 121    |
| DenseNet169    | 57 MB    | 0.762    | 0.932    | 14.3M    |  169    |
| DenseNet201    | 80 MB    | 0.773    | 0.936    | 20.2M    |  201    |

## Installation
This project has the following dependencies:

- Numpy `sudo pip install numpy`

- OpenCV Python `sudo apt-get install python-opencv`

- TensorFlow `sudo pip install --upgrade tensorflow-gpu`

- Keras `sudo pip install tf.keras` 

## Usage
To use this code, please ensure you have set up your dataset in folders following this structure:

    ├── "dataset_name"                   
    |   ├── train
    |   |   ├── class_1_images
    |   |   ├── class_2_images
    |   |   ├── class_X_images
    |   |   ├── .....
    |   ├── val
    |   |   ├── class_1_images
    |   |   ├── class_2_images
    |   |   ├── class_X_images
    |   |   ├── .....
    |   ├── test
    |   |   ├── class_1_images
    |   |   ├── class_2_images
    |   |   ├── class_X_images
    |   |   ├── .....

Then you can simply run `combined-model.py`.  
