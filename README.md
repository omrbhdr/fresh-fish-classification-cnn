# fresh-fish-classification-cnn

About Dataset
The dataset consists of a total of 40 images consisting of 20 images of fresh fish and 20 images of non-fresh fish.

Based on SNI 01-2729.1-2006, fresh fish has the following characteristics:
Pupils in black eyes stand out with clear corneas.

The gills are dark red and do not secrete mucus.
The meat is elastic (chewy) and dense when pressed.
Mucus on the surface of the skin is clear and colorless.
Meanwhile, non-fresh fish has the following characteristics:
The pupil of the eye looks very cloudy.
The color of the gills looks brown.
Has a soft meat texture.
Starting to smell bad.
The data acquisition process is carried out using a Samsung A6+ cellphone camera with a 4:3 (16MP) resolution 4608 x 3456 pixels which is placed in a static position as far as 10 cm.

After the data is obtained, preprocessing is carried out in the form of cropping the image to 500 x 500 pixels with a focus on the pupil of the fish eye, because based on the information above, the freshness of the fish can be identified by the pupil of the fish eye.

................................libs............................................

              import numpy as np
              import pandas as pd 
              import matplotlib.pyplot as plt
              from tensorflow import keras
              import os
              import cv2
              from sklearn import preprocessing
              from pathlib import Path
              from PIL import Image
              from tensorflow.keras.preprocessing.image import ImageDataGenerator
              from keras.models import Sequential
              from tensorflow.keras import layers
              from keras.layers import Dense, InputLayer, Dropout, Conv2D, MaxPooling2D, Flatten
              from keras.callbacks import EarlyStopping as ES
              from IPython.display import clear_output as cls
              from tensorflow.keras.layers import Conv2D,MaxPool2D,Dropout,Flatten,Dense,BatchNormalization
              import tensorflow as tf
              
.................................................................................

![image](https://github.com/omrbhdr/fresh-fish-classification-cnn/assets/12261537/1d76050b-a8dc-42cd-8cad-c65825088b61)
