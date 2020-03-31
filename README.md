# Optical Character Recognition
This project is concerned with Optical Chartacter Recognition consisting of four tasks; Recognising printed characters,
handwritten characters, to which person a signature belongs to and who wrote a handwritten letter between two people.

Two python files were created; "Extract Handwritten Letters" and "Extract Page", were both are used to extract letters from an image. The
first one is used to extract (as the name suggests) handwritten letters from a number of images and the other to extract printed letters
from a different list of images. The method both programs use is Sliding Window, were a window is formed that scans an image top-down and
left-to-right in order to detect a pixel intensity of non-ffffff. When the pixel intensity is detected, it checks the neighbours of that
part of the window in order to identify whether there are similar pixel intensities. Therefore, the program is able to form letters and extract
them as separate images. So in conclusion the programs were used in order to extract letters from images and form a dataset.

## Printed Character Recognition
Once letters were extracted and stored as separate images, they were loaded into a numpy array which was later split into training and testing.
The data was fed into a KNN classifier in order for it to train and be able to classify newly added images and extract words from them.

## Handwritten Character Recognition
This program served a similar purpose as the "Printed Character Recognition". For this case two machine learning algorithms were used
in order to experiment with them and identify which had a higher accuracy. The algorithms used were K-nearest neighbours and Support
Vector Machine. However, since the letters were handwritten, both models yielded a lower accuracy than the "Printed Character Recognition"
program did.

## Signature Recognition
The purpose of this program was to recognise to which person a signature belonged to. A custom dataset was created collecting signatures
from family members. Please note that the signature dataset is not included in this repository due to the sensitivity of the data.
Again, two machine learning algorithms were used; K-nearest neighbour and a Convolutional Neural Network. 

## Writed Identification System
Lastly, another program was developed were it would identify who wrote a certein letter between two people. Even though, it might had
been effective to use a binary classifier, a Convolutional Neural Network was used. The dataset created was a custom dataset of handwritten
letters (mine and a family member's). 

## Conclusion
This project was very effective in experimenting with Artificial Intelligence using different kinds of machine learning algorithms and
other technologies or methods such as k-fold cross-validation. Not only Insight knowledge was gained on how machine learning works, in particularly
optical recognition but a hands-on experience on building a system like that.

## Technologies and methods used
K-Nearest Neighbour

Support Vector Machine

Convolutional Neural Network

Numpy

Sckit-learn

Matplotlib

Keras 

Tensorflow

## How to run
This project can run on any notebook, I would suggest running it either on Google Colab or Jupyter.
Do note that file paths need to be changed.
