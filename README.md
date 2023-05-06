# Sign Language Classification README
This project aims to classify 25 of the English alphabet signs using a Convolutional Neural Network (CNN) model. The model was built using the Keras library and achieved an accuracy of 97.4% on the test set.

# Dataset
The dataset used in this project is the Sign Language MNIST dataset, which contains 27,455 grayscale images of size 28x28. Each image represents one of the 25 English alphabet signs (excluding J and Z) performed by a variety of signers. The dataset can be downloaded from this link.

# Model Architecture
The model architecture used in this project is a CNN with the following layers:

* Conv2D layer with 32 filters of size 3x3, input shape of (28,28,1), and 'relu' activation function
* MaxPooling2D layer with a pool size of 2x2
* Dropout layer with a rate of 0.25
* Conv2D layer with 64 filters of size 3x3 and 'relu' activation function
* MaxPooling2D layer with a pool size of 2x2
* Dropout layer with a rate of 0.25
* Conv2D layer with 128 filters of size 3x3 and 'relu' activation function
* MaxPooling2D layer with a pool size of 2x2
* Dropout layer with a rate of 0.25
* Flatten layer to convert the 2D feature maps into a 1D vector
* Dense layer with 512 units and 'relu' activation function
* Dense layer with 25 units (one for each class) and 'softmax' activation function
* Dropout layer with a rate of 0.25
The model was compiled using the 'categorical_crossentropy' loss function, 'adam' optimizer, and 'accuracy' metric.

# Training and Evaluation
The model was trained on the Sign Language MNIST dataset using a batch size of 512 and for 50 epochs. The training set was split into 80% for training and 20% for validation. The model achieved an accuracy of 97.4% on the test set.

# Conclusion
This project demonstrates the effectiveness of using CNN models for sign language classification tasks. The achieved accuracy of 97.4% on the test set shows that the model can accurately classify the English alphabet signs with high confidence.
