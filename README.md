# Hyperparameter tuning for classifying fashion product images with ResNet18


## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
This project focuses on enhancing the efficiency of a computer program designed to discern various types of fashion products depicted in images, such as clothing and accessories. The objective is to instruct the computer in distinguishing between different fashion items by fine-tuning its learning parameters, including the pace of learning and the degree of attention it allocates to specific details. The primary goal is to determine the optimal configuration for the computer's parameters, enabling it to achieve more effective recognition of fashion items within images. This project holds potential for applications in online retail platforms, ensuring accurate product recommendations, as well as facilitating fashion designers and retailers in the efficient organization of their product catalogues.

## DATA
The dataset I have chosen is called Fashion Product Images (Small) from Kaggle. This data was published on Kaggle by Param Aggarwal, and is sourced from a fashion e-commerce website in India: myntra.com.

In this dataset each product is identified by an ID such as 42431, and there is a map to all the products metadata in a csv file. This csv file contains the product ID, gender, primary category, secondary cateogry, type of clothing, colour, season, year, usage, and product display name. 

For this project, I will be using the images as the inputs for the model and secondary category as the outputs for the model.  

https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small


## MODEL 
I am using the ResNet18 model as it is a widely recognised model used for image classification tasks. It is also easily accessible through the torchvision.models library. 

## HYPERPARAMETER OPTIMSATION
The hyperparameters I chose to optimse included learning rate, momentum, weight decay, and optimiser type. I used Bayesian optimization through scikit-optimize to fine-tune these parameters within specified ranges. 
For the learning rate I chose to explore a range of values between 0.001 and 0.1 as this balances quick convergence without overshooting.
For momentum I chose to explore values between 0.1 and 0.9 to determine the optimal momentum for faster convergence.
For weight decay I explored values between 0.0001 and 0.01 to find the right balance between regularisation and model performance.
For the optimizer type I experimented with different optimization algorithms, including Stochastic Gradient Descent (SGD), Adam, RMSprop, and Nesterov Accelerated Gradient (NAG). Each optimizer type has unique characteristics and I aimed to identify which one works best for our specific task.

## RESULTS
A summary of your results and what you can learn from your model 

You can include images of plots using the code below:
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

