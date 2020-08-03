# sms-spam-detection-nlp-
* Import the nltk library
* Import the data and convert it into a pandas dataframe with message as one column and category as another column
* Perform some exploratory data analysis to recognize the kind of messages that are mostly classified as spam.(features such as message length can be used as a basis to classify messages into spam or ham)
* Now using some features of nltk library,such as stopwords and punctuation,convert these strings into a list of tokens(words that we actually want).
* Convert each message, represented as a list of tokens into a vector that machine learning models can understand.
   * Using Count-Vectorizer, we convert the list into a sparse matrix contatining the count of each word in each message.
   * Using TF-IDF,we can find out how important a word is in a document and generate a matrix of tf-idf weights.
* We can now use a machine learning model for training,I used Naive-Bayes classifier.
* Now split the data into training and test sets for testing purpose.
* We can now build a pipeline so that we don't have to type the lengthy code for pre-processing the testing data.
* Fit the testing data to the pipeline and make predictions.
* Check the accuracy of these predictions by using classification report(precision,recall,F1-score).
