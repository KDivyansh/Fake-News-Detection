Fake News Detection System that takes description of the news as input and returns if the news looks true or fake. Our Model has a 93.53% accuracy and trained on dataset of 7000+ rows. 

Requirements
To run this project, you'll need the following Python libraries:
  1. pandas
  2. scikit-learn
  3. nltk
  4. pickle
  5. re

This takes input as description and performs:
1. Data Preprocessing:
   1. Converts it into lower case
   2. Removes punctuation marks
   3. Removes stop words
   4. Tokenize the text
   5. Lemmatize the text
   6. And returns the preprocessed text.

2. Preparing Data:
   1. Allots dataframes to x and y
   2. Spliting data into x_train, x_test, y_train, y_test = train_test_split and returns the same

3. Vectorize Data
   1. Using TfIDF the text(tfid_x_train,tfid_x_test) is being vectorized.
   2. Returns the tfid_x_train and tfid_x_test

4. Model Training:
   1. For model training we have choosen PassiveAggressiveClassifier.
   2. It is not standard Classifier but it is mostly used in scam detection models. (Read More about this on : https://www.geeksforgeeks.org/passive-aggressive-classifiers/)

5. Evaluation of Model
   1.Evaluates the model's performance on the testing data
   2.Calculates the accuracy score, confusion matrix, and classification report

6. Saving and Loading the Model:
   1. Saves the trained model to a file using pickle
   2. Loads the saved model from the file
  
7. Predicting News:
   1. Takes a news article text as input
   2. Preprocesses the text
   3. Vectorizes the text using the same TF-IDF vectorizer
   4. Predicts whether the news is fake or real using the loaded model
  

HOW TO RUN:
1. pip install -r requirements.txt
2. python Fake_News_Det.py
   
