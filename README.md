# Text-Review-to-Rating-Stars-Transformer
Using Machine Learning techniques, we create a model that provides a text input (eg. a review for a restaurant) and gives a rating in the form of [1-5] stars.

-data: includes a pkl file with tf-idf results, a stopwords file and a dictionary that is used for the glove.
* the stopwords are the ones that keras contains, except for those with negative meaning (eg. not, haven't, isn't etc)
** pkl files is not included due to its size (500MB). It can be reproduced using the code.

- data analysis: contains the files used for the graph and map creation.

- tools: contains scripts for the stopwords' processing, an encoder in order to have the models in a compatible form for the kerasJs and a server that starts an api for the case that we need a way to run the models.

- main.py file with which the project is started.

- svm_classification implements instances classification with svm.

- yelp_neural_networks.py contains two neural networks (lstm, cnn) 

- attention.py, combined with the previous one .py file, creates an lstm with attention layer.

- html folder contains the web page with the results

