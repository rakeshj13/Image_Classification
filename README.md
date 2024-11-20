Overview
This project demonstrates the use of Convolutional Neural Networks (CNNs) to classify images from the CIFAR-10 dataset into 10 distinct categories:
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.

The project compares the performance of a basic Artificial Neural Network (ANN) with a CNN model and highlights the superior accuracy of CNNs for image classification tasks.

Dataset
The CIFAR-10 dataset consists of 60,000 32x32 color images divided into 10 categories.

Training Set: 50,000 images
Test Set: 10,000 images
Each image is labeled with one of the 10 classes.

Project Workflow
Data Loading and Preprocessing

The dataset is loaded using TensorFlow's datasets.cifar10 module.
Images are normalized by scaling pixel values to the range [0, 1].
ANN Model

A basic Artificial Neural Network with dense layers is implemented.
Achieved ~49% accuracy on the test set.
CNN Model

A Convolutional Neural Network is implemented with the following architecture:
2 Convolutional Layers with MaxPooling
Flatten layer
Fully connected Dense layers with ReLU and Softmax activation functions
Achieved ~70% accuracy on the test set, outperforming the ANN.
Evaluation

Models are evaluated using metrics like accuracy, precision, recall, and F1-score.
Confusion matrices and classification reports provide detailed performance insights.
Results
Model Type	Test Accuracy
ANN	~49%
CNN	~70%
