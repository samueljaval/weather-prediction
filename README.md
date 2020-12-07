# weather-prediction

This project was made for the Scientific Computing Class (COMP260) at Wesleyan University. 

Our project needed three areas of focus picked from everything we studied throughout the semester. 
My three areas of focus are : 
- Timeseries analysis 
- Scikit Learn 
- TensorFlow 

The goal of this project was to look at what someone with a good programming and computer science background but with almost no data science background should do to make a simple temperature predictor. The main question here was should we implement a simple Linear Regression or use a Deep Neural Network? 

The project contains 4 files : 
- getData.ipynb (I didn't want to use a pre-made dataset that I could find online (on Kaggle for example) so I used the online weather API to get my data) 
- linearRegression.ipynb (We predict the temperature with a Linear Regression using the Scikit Learn Python Library) 
- deepNeuralNetwork.ipynb (We predict the temperature with a deep Neural Network using the TensorFlow High Level API) 
- extended_data.csv (this file contains the data we got from getData.ipynb if one does not want to run the script again, we see in getData.ipynb why it's called "extended") 

Our Linear Regression predicted the temperature with an accuracy of about 92% and the Deep Neural Network predicted with an accuracy of about 93%. The results are therefore realtively similar and after having gone through implementing both models I can say that implementing the Linear Regression might have been a little easier. However, Deep Neural Networks are very powerfull and a full optimization by fine tunning every single parameter could potentially have led to a way better model than the Linear Regression. If I had the opportunity to improve this project I would conduct deeper research on how I can fine tune the parameters to get a better result from the deep neural network. I could maybe also try to implement another type of model from the TensorFlow Library that doesn't use the High Level API and would allow more control over what is going at a slighly lower level.
