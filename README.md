## Dog Breed Classifier


Ever looked at a dog and wondered what breed that dog was? Well I certainly have. So I decided to train an Image Classification model that would return the breed of a dog when given an image. 

The Dataset used to train this model can be found on Kaggle in the following link: https://www.kaggle.com/c/dog-breed-identification

This is a machine learning model built using a Convolutional Neural Network paired with Transfer Learning. Essentially, it is a sort of pseudo-base-head pair. The base is made up of three pretrained models:
1. Xception
2. Inception V3
3. Inception ResNet V2

We pass in the training data to each pretrained model. The model produces a corresponding feature map which is saved in a variable. Then the three feature map are concatenated together and passed into our custom made head which returns an array containing the predictions of the model. 
