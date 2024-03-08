# Fake-News-Detection
Detecting fake news using Long Short Term Memory (LSTM).

This repository contains code for detecting fake news articles using Long Short-Term Memory (LSTM) neural networks. The model is trained on a dataset of labeled news articles to classify them as either real or fake.

Dataset
The dataset used for training and evaluation is the Fake News Dataset which consists of a collection of news articles labeled as real or fake. It contains features such as article text, title, and others. I perfomed data cleaning in which we removed the NEWS that have unkown publishers and than I perfomed data preprocessing by converting data to the lowercase after that I created new column with the name class in which I assign 1 to true news and to fake after that I also remove special characters. After preprocessing I vectorized word to tokens using gensim and than use this data in tensorflow/keras Long Short Term Mermory (LSTM) to create model that detect fake news.
