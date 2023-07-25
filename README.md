# ABSTRACT
This project focuses on implementing Object Detection (Sign Language Detection) model, using TensorFlow. By utilizing our webcam, we collect images of different signs and label them using 'LabelImg.' Next, we employ the Transfer Learning approach with the TensorFlow Object Detection API, using SSD MobileNet for training. The result is real-time sign language detection through Python and openCV, enabling the identification of sign language poses via the webcam. 

# STEPS TO BUILD THE MODEL

## 1. Installation and Setup:
Install the required software, tools, packages, and clone the necessary GitHub repositories by referring to the 'Installation and Setup' section above for detailed guidance.
Link - https://github.com/ramgopalputta/Sign_Language_Detection_Using_TensorFlow/blob/main/Installation%20and%20Setup

## 2. Collecting the images and labelling them using 'LabelImg':
We will be using our own webcam to collect the images of various signs and then pass them to 'LabelImg', which is is a graphical image annotation tool.
Make sure to keep your object detection bounding box as tight as possible, include pictures from various angles and lighting conditions, and begin with 10-20 images per class.

<img src="![Victory_cropped](https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/45c73931-76e2-4f59-879a-5c8b52013cfb)" width="400" height="400" />


![Thumbsdown_cropped](https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/6f8bc2db-ab96-4e3a-91cc-6106bba39119)



## 2.  Training TensorFlow Object Detction Models:
Now, we are going to use Transfer leraning approach against the TensorFloe object detection API using SSD MobileNet

### Freezing and Conversion

### Performance Tuning

## 3. Detecting sign language in real time using Webcam:
Finally, using python and openCv, real time sign language poses are detected via your webcam. 




