# chatbot
Python NLTK, Chatbot using tensorflow, keras, and Natural Language Tool Kit
Hi, this project was inspired from "Shivashish Thkaur" link can be found here https://dzone.com/articles/python-chatbot-project-build-your-first-python-pro
In order to understand the project properly we have to determine the usage of various libraries, in the training module:
the libraries we have to import:
import numpy as np
from keras.models import Sequential
from keras.layers import Dense, Activation, Dropout
from keras.optimizers import SGD
import random

import nltk
from nltk.stem import WordNetLemmatizer
lemmatizer = WordNetLemmatizer()
import json
import pickle
1) Keras functions are imported under tensorflow library:
they are used to integrate our training set, for the chatbot. 
Optimizer function, to calculate the epochs and determine the accuracy of the data
Layers, are meant to implement the primary layers and shapes of tensors. Depending on the dataset we determine the dense of keras.
2) Numpy is used to take the arrays and use them under different functions, to fit in our model
3) we use pickle to open our txt files, and change their values.

One of the initial steps we take towards this project is to create 
lists that will store some of the columns we need under our json file, also to get 
rid of some the syntaxes we do not require to train
all of our intents are designed to store the questions and responses of our ai. 
In this case we store them under different classes(tag), patterns(user inputs), 
and responses(ai chatbot). 

