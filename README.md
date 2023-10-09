# Creating a sequential model through hyperparameter tuning for classifying fashion product images


## Non-technical explanation of the project

This project focuses on improving the accuracy of a computer program designed to classify fashion product images, such as clothing. The goal is to enhance the program's ability to distinguish between various fashion items by fine-tuning key parameters, including the size of input layers, choice of activation functions, and the learning rate of the optimizer. The primary objective is to determine the optimal configuration for these parameters, enabling more effective recognition of fashion products within images. This project has practical applications in e-commerce for accurate product categorization and recommendation, aiding fashion designers and retailers in efficiently organizing their product catalogue.

## Data

The dataset utilized for this project is Fashion MNIST, a popular benchmark dataset in the field of computer vision. Fashion MNIST consists of grayscale images of fashion items, each belonging to one of ten categories, including items like T-shirts, dresses, and shoes.


## Model

This project constructs a custom Sequential model for this task. This Sequential model is a stack of one flattened input layer and four dense layers the last of which is the output layer. The first three dense layer's architecture, including the number of neurons and activation functions, is determined through hyperparameter tuning. The goal is to find the most effective combination of these hyperparameters for accurate classification.

## Hyperparameter Optimisation

The following hyperparameters are tuned:

Dense Layer Sizes: The number of neurons (units) in each of the three dense layers is a critical factor affecting the model's capacity to learn complex patterns. Through hyperparameter tuning, we explore different configurations for these layer sizes to determine the optimal combination.

Activation Functions: The choice of activation functions for each dense layer significantly impacts the model's ability to capture intricate features in the data. The hyperparameter tuning process investigates various activation functions, such as ReLU and tanh, for each dense layer to identify the most effective combination.

Learning Rate: The learning rate is a key hyperparameter governing the step size during model training. We conduct hyperparameter tuning to find the optimal learning rate value that ensures rapid convergence without overshooting.

By systematically exploring and optimizing these hyperparameters, the project aims to create a custom Sequential model that excels in classifying fashion product images within the Fashion MNIST dataset.

## Results
A summary of your results and what you can learn from your model 

You can include images of plots using the code below:
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

