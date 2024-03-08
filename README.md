# Fake-News-Detection
Detecting fake news using Long Short Term Memory (LSTM).

This repository contains code for detecting fake news articles using Long Short-Term Memory (LSTM) neural networks. The model is trained on a dataset of labeled news articles to classify them as either real or fake in 
python.

Dataset
The dataset used for training and evaluation is the Fake News Dataset which consists of a collection of news articles labeled as real or fake. It contains features such as article text, title, and others. I perfomed data cleaning in which I removed the NEWS that have unkown publishers and than I perfomed data preprocessing by converting data to the lowercase after that I created new column with the name class in which I assign 1 to true news and to fake after that I also remove special characters. After preprocessing I vectorized word to tokens and apply padding of 1000 for each sentences using gensim and than use this data in tensorflow/keras Long Short Term Mermory (LSTM) to create model that detect fake news. In model I have used Embedding layer (that is used to represent words), LSTM layer (that is used in place of SImpleRNN to avoid short term memory) and than Dense layer. 

![image](https://github.com/muhammadmehdi89/Fake-News-Detection/assets/142395586/5dbd5b47-adcb-48a3-88e5-54e66599930c)

I Have Got Excellent Validation and Test Accuracy:

![image](https://github.com/muhammadmehdi89/Fake-News-Detection/assets/142395586/1957f8f7-0a40-466e-b042-903bd77fdf91)

## Classification report:

![image](https://github.com/muhammadmehdi89/Fake-News-Detection/assets/142395586/b9f6637a-ffdf-4efb-bdc9-936d8e96fdf0)

Requirements
TensorFlow 2.x
Keras
Pandas
NumPy
NLTK (Natural Language Toolkit)
gensim.

