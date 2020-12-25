# Face-Recognition-Model

## Table of Contents
+ [About](#about)
+ [Applications](#Applications)
+ [Technical System Architecture](#technical-system-architecture)
+ [Results](#results)
+ [References](#references)
+ [Installations](#installations)

## About
Facial recognition  biometric tool that  recognizing a human face from the database of known faces  A facial recognition system uses biometrics to map facial features from a photograph or video. 

Facial Recognition Technology has been around for decades. How ever in recent years its is seen as wide spread adoption mainly because of Artificial intelligence advances deep learning in faster systems for processing the enormous amount of data. It helps the technology composure to reaching it for potential .This has lead to higher accuracy and faster processing times. Government and private companies  are taking notice in Face Recognition Technology.

The facial recognition market is expected to rise by $12.92 billion in 2027. That’s because facial recognition has all kinds of commercial applications. It can be used for everything from surveillance to marketing.

# Applications:
Perform secure transactions with contactless transactions.<br>
Identify people in social media.<br>
Recognize thieves. <br>
Help blind people for recognizing the people.<br>
Find Missing Persons. <br>
Aid Forensic Investigations<br>
Attendance Management systems. etc.

## Technical System Architecture
| Stages| Face Detection | Face Alignment  |Face Feature <br>Extraction|Face Classification|
| --- |-------------| -----|-----|-----|
|**ML Models**|||**facenet_keras.h5** <br>*(Identity)*<br>| SoftMax Classifier |
| **Libraries**| Dlib|imutils|Keras<br>TensorFlow |Scikit Learn |
|**Language**| Python|Python|Python|Python|

## Results

<img src="https://github.com/GangababuManam/FaceRecognition/blob/main/Test.jpg" width="300" height="300">


We have trained the system with some of my friends.We have used 3 photos per person with clean, clear, front facing faces would produce better results for identity estimates. 

The Softmax classifier is also prefered over SVM,KNN classifier as they produce slightly better estimation. It also provides a confidence score per estimate which allows us to set a threshold to categorize known or new faces. The confidence score threshold we experimented that works best is 0.9.

Model was tested on both faces with glasses and without glasses and model worked in both cases perfectly. 

## References
<br>Face Detection: [DLib](http://dlib.net/)
<br>Face Alignment: https://github.com/jrosebr1/imutils/blob/master/imutils/face_utils/facealigner.py
<br>Face Recognition Models: https://machinelearningmastery.com/how-to-develop-a-face-recognition-system-using-facenet-in-keras-and-an-svm-classifier/

## Installations
To run the model, please install the required python packages using
```
pip install -r requirements.txt
```
```


**To train new faces for face identification:**<br>
Import photos to `faces/name_of_person/001.jpg` and run the codes again.
