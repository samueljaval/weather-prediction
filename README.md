# weather-prediction

### Notes

1. Every `.ipynb` file is **thoroughly** commented to help the reader understand the thought process.
2. Github's IPython Notebook viewer is sometimes buggy so if you can't look at the files here, you can follow these links : 
    - https://colab.research.google.com/github/samueljaval/weather-prediction/blob/main/getData.ipynb
    - https://colab.research.google.com/github/samueljaval/weather-prediction/blob/main/linearRegression.ipynb
    - https://colab.research.google.com/github/samueljaval/weather-prediction/blob/main/deepNeuralNetwork.ipynb

### The Project
This project was made for the Scientific Computing Class (COMP260) at Wesleyan University and is focused on three specific topics : Timeseries analysis, Scikit Learn, and TensorFlow. The main goal of the project was to show the pros and cons of implementing a simple Linear Regression or a Deep Neural Network for a temperature prediction model. 

### Content
The project contains 4 files: 
- **getData.ipynb** : 
This is where I collected the data to train my models later on. I didn't want to use a pre-made dataset that I could find online - on Kaggle for example - so I used the online weather API to get my data. The API limits the amount of data we can collect per GET request, therefore I had to do a little bit a scripting to automate making numerous requests for the amount of data I wanted. I collected daily weather data (e.g avg temp, wind speed, humidity, ...) from January 1st 2009 to December 31st 2019 from a specific location in France (Val D'Isère). I also had to do a little more scripting after getting all the data to clean it and have it in a desired format. I put the data in a pandas dataframe since it is well suited for the libraries I used to create my models. I then stored that dataframe in a .cvs file so that I could import it into the other files of the project.

- **linearRegression.ipynb** : In this file, I tried to predicts the temperature with data from the 3 previous days using a simple Linear Regression model. I used the Scikit Learn Python Library for my Linear Regression. Before feeding the data to the model, I did some analysis to filter out weather features that appeared to not be correlated to temperature. 

- **deepNeuralNetwork.ipynb** : In this file, I tried to predicts the temperature with data from the 3 previous days using a Deep Neural Network. I used TensorFlow's High Level API. My Deep Neural Network has two hidden layers with 25 nodes each and the activation function is the Rectified Linear Unit (ReLU). 

- **extended_data.csv** : This file contains the data we got from getData.ipynb. 

### Results and Analysis
The Linear Regression predicted the temperature with an accuracy of about 92% and the Deep Neural Network predicted with an accuracy of about 93%. The results are therefore relatively similar. After implementing both models I can say that implementing the Linear Regression is a little easier and it ran a lot faster than the Deep Neural Network (1 or 2 sec vs. a couple minutes). However, Deep Neural Networks are very powerfull and a full optimization by fine tunning every single parameter could potentially have led to a way better model than the Linear Regression. If I had the opportunity to improve this project I would conduct deeper research on how I can fine tune the parameters to get a better result from the deep neural network. I could maybe also try to implement another type of model from the TensorFlow Library that doesn't use the High Level API and would allow more control over what is going at a slighly lower level.

I thank Professor Thayer for making this class feel normal in this very abnormal semester. 
