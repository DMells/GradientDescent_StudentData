# Training a neural network example
This neural network looks at three parameters of student performance data and makes a prediction of whether or not they get admitted to a university. The parameters influencing the acceptance is the student's GRE score, the GPA, and a 1-4 ranking of the education establishment itself. The last is particularly interesting because it is categorical data, and so each rank is split out into it's own column prior to training the network.

This repository contains three core files, and a requirements.txt file:
1. Gradient.py performs the forward and backward passes through the network
2. Data_prep.py splits the data into a training and test set and fixes the categorical issue above
3. binary.csv student raw data

The data was taken from http://www.ats.ucla.edu/stat/data/binary.csv

This exercise is concerned with implementing gradient descent into a neural network, i.e. the key element of the backwards propogation technique which serves to tweak the (initially random) weights of the activation function (from the forward pass). 

In doing so we seek to minimise the error by adjusting the weights of our prediction function such that we move down the negative of the gradient of the error function, and consequently improving the fit of our prediction function to the actual data.

The output is a trained network, and the accuracy is displayed when running the gradient.py file in your terminal. 

For convenience I have uploaded my anaconda virtual environment setup (using python 3.6) so you can install and get started straight away (requirements.txt)

From training the model, we obtain a 72.5% prediction accuracy i.e. the likelihood that based on the three data types we can predict whether or not a student will get accepted with a 72.5% accuracy.
