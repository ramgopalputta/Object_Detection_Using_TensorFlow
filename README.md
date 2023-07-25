# ABSTRACT
This project focuses on implementing Object Detection (Sign Language Detection) model, using TensorFlow. By utilizing our webcam, we collect images of different signs and label them using 'LabelImg.' Next, we employ the Transfer Learning approach with the TensorFlow Object Detection API, using SSD MobileNet for training. The result is real-time sign language detection through Python and openCV, enabling the identification of sign language poses via the webcam. 

# STEPS TO BUILD THE MODEL

## 1. Installation and Setup:
Install the required software, tools, packages, and clone the necessary GitHub repositories by referring to the 'Installation and Setup' section above for detailed guidance.
Link - https://github.com/ramgopalputta/Sign_Language_Detection_Using_TensorFlow/blob/main/Installation%20and%20Setup

## 2. Collecting the images and labelling them using 'LabelImg':
Using a webcam, images of various signs are collected and passed to 'LabelImg', a graphical image annotation tool (https://github.com/HumanSignal/labelImg). \
Ensure tight object detection bounding boxes, include pictures from different angles and lighting conditions, and start with 10-20 images per class.

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/47c85a39-40e1-403c-8abc-2cae9e4bd40b" width="200" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/262cedb1-ffb1-49f8-9b89-2cbc37b2ea4a" width="200" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/99de80f6-515c-4241-a1f3-f042ccae2203" width="200" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/70022a6e-2498-4198-8794-da3f1444a0c1" width="200" height="250" />

## 2.  Training TensorFlow Object Detction Model:
Now, a Transfer learning approach will be utilized against the TensorFlow object detection API using SSD MobileNet.\
Pretrained model used: ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8
https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md.

### Evaluation
Once the model is trained, the model is evaluated by determinig: \
Mean Average Precision - TP/(TP+FP) - what proportion of detections were correct? (Ideally, As high as possible)\
Mean Average Recall    - TP/(TP+FN) - what proportion of actual objects were captured?\
Loss - Evaluating how well the model is performing against the given data.\
Ideally, Precision and Recall must be as high as possible; and Loss should be low.


## 3. Detecting sign language in real time using Webcam:
Finally, using python and openCv, real time sign language poses are detected via your webcam. 


## 4. Performance Tuning
Performance Tuning is a set of optimizations and best practices which can accelerate training and boosts the performace of deep learning models.
This can be achieved by:
* Adding more images to the traning set particularly for low-performing classes, and varying backgrounds and lighting conditions, etc..
* Trainig longer by increasing the number of epochs.
* Changing the model architecture.


