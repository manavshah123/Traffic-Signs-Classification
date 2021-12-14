# Traffic-Signs-Classification

<h2> 1.	Introduction</h2>
This case study is designed to Classify the traffic signs. It uses the Sequential and ResNet model for the images. The model built is able to grid the image and train model accordingly and then predict the sign from them.
This case study can be used across various sectors where there is a need to have the Traffic sign classification. Also, if this model is trained with more resources like GPU, RAM then it can be expanded to cover variety of traffic signs categories.

<h2> 2.	Tools and Technologies</h2>

Tools and Libraries	Usage
Keras	
Sequential
matplotlib
Kaggle

<h2> 3.	Model Explanation and Architecture </h2>

ResNet, short for Residual Networks is a classic neural network used as a backbone for many computer vision tasks. This model was the winner of ImageNet challenge in 2015. The fundamental breakthrough with ResNet was it allowed us to train extremely deep neural networks with 150+layers successfully. Prior to ResNet training very deep neural networks was difficult due to the problem of vanishing gradients.

<img src="https://github.com/manavshah123/Traffic-Signs-Classification/blob/main/resnet50.png"/>

<h2> 4.	Working </h2>

The images we use daily contains multiple traffic signals The values of these channels can vary from 0 to 255. While training the model, we use the traffic signals images here we define the number of classes is 43 and number of channels is 3 and a s preprocessing we have to resize the image in 224 * 224 format. In the project dence layer activation is “softmax” and objective function is categorical_crossentropy ( Used as a loss function for multi-class classification model )  

Here we define number of epoch is 10, and the  early stop  patience is  3 and  now we have to load dataset  and pickle file

Now Preparing y_train and y_validation for using in Keras num_classes: Total number of classes. If nothing is mentioned, it considers the largest number of the input vector and adds 1, to get the number of classes.Its default value is "None". 

And then we have to convert all sample images into the grid and plot them for better understanding, then we have to train our model and test it with some input images of traffic signals.

<h2> 5.	Output </h2>

<img src="https://github.com/manavshah123/Traffic-Signs-Classification/blob/main/output.png"/>
