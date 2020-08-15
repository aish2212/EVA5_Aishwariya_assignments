# ASSIGNMENT 4

# Objective
Train MNIST Dataset and achieve 99.4% validation accuracy with the following restrictions:
 - Less than 20k Parameters
 - You can use anything from above you want. 
 - Less than 20 Epochs
 - No fully connected layer

# Model
The neural network architecture is as follows:
- input image size is 28 * 28
- The network contains 3 convolutional nested layers.
- 1st convolutional nested layer (conv1) have 3 convolutional layer.
- 1st conv1 is followed by MaxPool.
- 2nd (conv2) and 3rd (conv3) convolutional nested layer have 2 convolutional layer each.
- Each convolution layer is followed by activation function (RELu).
- Each activation function is followed by batch-normalization.
- Each batch-normalization is followed by dropout.
- After the 3rd convolution (conv3) we have global average pooling (GAP)
- Then the final softmax layer.

# Features
- The total parameters used in the models is 17,200.
- Batch Size = 64
- Learning rate = 0.01
- Drop-out = 0.1

# Final Output
- The model has test accuracy of 99.49% maximum at the 15th epoch

