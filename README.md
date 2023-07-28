# Text Classification using Naive Bayes

This repository contains Python code for text classification using the Naive Bayes algorithm. The project aims to perform text classification on the 20 Newsgroups dataset and includes two implementations of Naive Bayes - one using `scikit-learn` and the other from scratch.

## Dataset
The 20 Newsgroups dataset is used for this project. It is a collection of newsgroup documents, partitioned into 20 categories. The dataset is divided into training and test sets.

## Dependencies
1. numpy
2. scikit-learn
3. nltk
4. matplotlib

## Implementation Details

### Part 1: Text Classification using Multinomial Naive Bayes (Sklearn)
The `MultinomialNB` class from `scikit-learn` is utilized to perform text classification using the Naive Bayes algorithm. The text data is preprocessed by removing stopwords, punctuation, and non-alphabetic characters. The top 10,000 words with the highest frequency are selected as features. The training and test data are modified to represent the frequency of these features, and the `MultinomialNB` model is trained and evaluated on the test set.

### Part 2: Custom Naive Bayes Implementation
A custom implementation of the Naive Bayes algorithm is built from scratch for text classification. The `NaiveBayes` class includes methods to fit the model on training data and predict class labels for test data. The `fit` method calculates word frequencies for each class and stores the relevant information. The `predict` method utilizes these frequencies to predict class labels for the test set.

## Results
The accuracy and performance metrics of both implementations are compared and presented. The custom Naive Bayes implementation's accuracy is compared with the Sklearn version. The classification report and confusion matrix are provided to evaluate the model's performance for each class.

## How to Use
1. Install the required dependencies mentioned above.
2. Run the provided code to perform text classification using both Sklearn and custom Naive Bayes implementations.
3. Analyze the accuracy and performance metrics for the text classification task on the 20 Newsgroups dataset.

Feel free to explore the code, experiment with different datasets, and make improvements to the Naive Bayes algorithm for text classification. Enjoy the project!
