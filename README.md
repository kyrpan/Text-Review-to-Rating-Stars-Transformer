# Text-Review-to-Rating-Stars-Transformer
Using Machine Learning techniques, we create a model that provides a text input (eg. a review for a restaurant) and gives a rating in the form of [1-5] stars. 

We use the dataset provided from Yelp containing reviews for restaurants, in order to train our models. At the preprocessing stage, we remove stopwords, punctuation and numerical digits. Then we tokenize the text and create a vocabulary with the 80.000 most frequent words. Each word is mapped to an integer. Finally, in each review we replace each word with its mapped integer.

Concerning the models, we set up two Neural Networks: a CNN and an LSTM. The first one reached an accuracy of 60.5% while the second one made it to 62.4%.

- data: includes a pkl file with TF-IDF results, a stopwords file and a dictionary that is used for the glove.

* the stopwords are the ones that keras contains, except for those with negative meaning (eg. not, haven't, isn't etc)

** pkl files is not included due to its size (500MB). It can be reproduced using the code.

- data analysis: contains the files used for the graph and map creation.

- tools: contains scripts for the stopwords' processing, an encoder in order to have the models in a compatible form for the kerasJs and a server that starts an api for the case that we need a way to run the models.

- main.py file starts the project.

- svm_classification implements instances classification with SVM.

- yelp_neural_networks.py contains two neural networks (LSTM, CNN) 

- attention.py, combined with the previous .py file, creates an LSTM with attention layer.

- html folder contains the web page with the results

