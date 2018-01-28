# CS 671 Project

Project uses different Deep Learning and Machine Learning Models to create a substanital dataflow to automate media(tweets and text) generation.

#Dataflow and the Models working at those levels is as follows:
## Tweeter API to get the tweets about any event
### This gets the data from the people around the world regarding any event one wants 
## Vector Representation of Words and Documents and Tf-Idf scores
### The tweets are given to the word2vec and doc2vec models of Ginsim to generate vector representations of the tweets and also finding the tf-idf scores
## Sentiment Classification of the tweets using feed forward Neural network
### For classification, word embeddings in conjunction with the tf-idf scores are used. The vector of words is constructed by multiplying the word embeddings and the corresponding tf-idf scores, which in effect give us weighted average of all the word vectors available in the tweet. Then we divide the dataset into training and testing dataset and train a simple two layer feed-forward network, with one hidden layer and one output layer.
## Time series for Sentiment Fluctuations during the duration of the event
## Text or tweet generation 
### Recurrent Neural Networks are used for tweet generation. The Long Short Term Memory(LSTM) cells are used in the neural network, with a single layer 