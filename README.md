# weather-prediction

This project was made for the Scientific Computing Class (COMP260) at Wesleyan University. 

The three areas of focus for this project are : 
- Timeseries analysis 
- Scikit Learn 
- TensorFlow 

The main goal here was to show the pros and cons of implementing a simple Linear Regression or a Deep Neural Network. 

The project contains 4 files (The .ipynb are thoroughly commented to help the reader understand what we are doing): 
- getData.ipynb (I didn't want to use a pre-made dataset that I could find online - on Kaggle for example - so I used the online weather API to get my data) 
- linearRegression.ipynb (the temperature is predicted with a Linear Regression using the Scikit Learn Python Library) 
- deepNeuralNetwork.ipynb (the temperature is predicted with a deep Neural Network using the TensorFlow High Level API) 
- extended_data.csv (this file contains the data we got from getData.ipynb, we see in getData.ipynb why it's called "extended") 

Our Linear Regression predicted the temperature with an accuracy of about 92% and the Deep Neural Network predicted with an accuracy of about 93%. The results are therefore relatively similar. After having gone through implementing both models I can say that implementing the Linear Regression is a little easier and it ran a lot faster than the Deep Neural Network (1 or 2 sec vs. a couple minutes). However, Deep Neural Networks are very powerfull and a full optimization by fine tunning every single parameter could potentially have led to a way better model than the Linear Regression. If I had the opportunity to improve this project I would conduct deeper research on how I can fine tune the parameters to get a better result from the deep neural network. I could maybe also try to implement another type of model from the TensorFlow Library that doesn't use the High Level API and would allow more control over what is going at a slighly lower level.

The class readings and discussions played a very important role in my understanding of these topics (especially on Deep Neural Networks) and made it a lot easier to implement and comprehend the models.

I thank Professor Thayer for making this class feel normal in this very abnormal semester. 
