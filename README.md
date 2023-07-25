# 1. ABSTRACT
This project focuses on implementing Object Detection (Sign Language Detection) model, using TensorFlow. By utilizing our webcam, we collect images of different signs and label them using 'LabelImg.' Next, we employ the Transfer Learning approach with the TensorFlow Object Detection API, using SSD MobileNet for training. The result is real-time sign language detection through Python and openCV, enabling the identification of sign language poses via the webcam. 

# 2. INSTALLATION AND SETUP:

Install the required software, tools, packages, and clone the necessary GitHub repositories by referring to the 'Installation and Setup' section above for detailed guidance.
Link - https://github.com/ramgopalputta/Sign_Language_Detection_Using_TensorFlow/blob/main/Installation%20and%20Setup

### _1. Python using Anaconda_
Install a python version using Anaconda, to run TensorFlow within the Jupyter notebook.

Installation link:
https://repo.anaconda.com/archive


### _2. Microsoft Visual Visual C++_
TensorFlow necessitates C++ Build tools, and CUDA requires Visual Studio.

Installation link:
https://visualstudio.microsoft.com/vs/community/


### _3. CUDA and CUDNN for NVIDIA_
If you are using an Nvidia GPU, you need to install CUDA and CUDNN to accelerate the Deep learning process and training.

Check the versions of Tensorflow_gpu from the below link and install the corresponding CDA and CUDNN:
https://www.tensorflow.org/install/source_windows

CUDA installation link:
https://developer.nvidia.com/cuda-11.2.0-download-archive

CUDNN installtion link:
https://developer.nvidia.com/rdp/cudnn-archive


### _4. Protocol Buffers_
These are the formats that the TensorFlow saves the model in. TensorFlow graphs are represented in a format called protocol buffer.

Install Protoc for Protocol Buffers from the below official Github Repo link:
https://github.com/protocolbuffers/protobuf/releases


### _5. GIT Bash_
This allows us to use Git commands.

Installation link:
https://git-scm.com/downloads


### _6. Tensorflow Object Dtection API_
The TensorFlow Object Detection API is a open-source framework, developed on TensorFlow. It helps to build, train, and deploy the object detection models. The framework includes pre-trained models, referred to as the Model Zoo.

Clone the below github repo:
https://github.com/tensorflow/models

# 3. COLLECTING THE IMAGES AND LABELLING THEM USING 'LABELIMG'
Using a webcam, images of various signs are collected and passed to 'LabelImg', a graphical image annotation tool (https://github.com/HumanSignal/labelImg). \
Ensure tight object detection bounding boxes, include pictures from different angles and lighting conditions, and start with 10-20 images per class.

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/47c85a39-40e1-403c-8abc-2cae9e4bd40b" width="200" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/262cedb1-ffb1-49f8-9b89-2cbc37b2ea4a" width="200" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/99de80f6-515c-4241-a1f3-f042ccae2203" width="200" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/70022a6e-2498-4198-8794-da3f1444a0c1" width="200" height="250" />

# 4. TRAINING TENSORFLOW OBJECT DETCTION MODEL
Now, a Transfer learning approach will be utilized against the TensorFlow object detection API using SSD MobileNet.\
Pretrained model used: ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8
https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md.

# 5. MODEL EVALUATION
Once the model is trained, the model is evaluated by determinig: \
Mean Average Precision - TP/(TP+FP) - what proportion of detections were correct? (Ideally, As high as possible)\
Mean Average Recall    - TP/(TP+FN) - what proportion of actual objects were captured?\
Loss - Evaluating how well the model is performing against the given data.\
Ideally, Precision and Recall must be as high as possible; and Loss should be low.


# 6. DETECTING SIGN LANGUAGE IN REAL TIME, USING WEBCAM
Finally, using python and openCv, real time sign language poses are detected via your webcam. 

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/38e40d73-a4a1-4398-a8a3-6c024cf3289c" width="225" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/9eed0334-e091-4f87-aee1-d409a59ac869" width="225" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/6fd8e5cd-b206-4879-998b-bbdce3fdab99" width="225" height="250" />

<img src="https://github.com/ramgopalputta/Object_Detection_Using_TensorFlow/assets/114395443/f579d1f8-9f36-4ae2-bbeb-9dd460d1c7e3" width="275" height="250" />



# 7. PERFORMANCE TUNING
Performance Tuning is a set of optimizations and best practices which can accelerate training and boosts the performace of deep learning models.
This can be achieved by:
* Adding more images to the traning set particularly for low-performing classes, and varying backgrounds and lighting conditions, etc..
* Trainig longer by increasing the number of epochs.
* Changing the model architecture.


