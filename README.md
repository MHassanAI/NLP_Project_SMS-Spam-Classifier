# SMS Spam Classifier

This project implements an SMS spam classifier using machine learning techniques. The classifier is built using Python and various libraries such as `nltk`, `pandas`, `scikit-learn`, and more.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)

## Introduction

The goal of this project is to classify SMS messages as either spam or ham (not spam). This is achieved by training a Naive Bayes classifier on a labeled dataset of SMS messages. The classifier preprocesses the text messages, extracts features using TF-IDF, and then applies the model to predict the labels.

## Dataset

The dataset used in this project is the `SMSSpamCollection` file, which contains SMS messages labeled as spam or ham. Each line in the file is a tab-separated entry with two fields:
- `Label`: 'spam' or 'ham'
- `Message`: The content of the SMS

## Dependencies

To run the code in this repository, you will need the following Python libraries:
- `nltk`
- `pandas`
- `numpy`
- `scikit-learn`

You can install these dependencies using `pip`: pip install nltk pandas numpy scikit-learn

## Model Training and Evaluation

The script performs the following steps:

- Text Preprocessing: Cleans the text by removing non-alphabet characters, converting to lowercase, lemmatizing, and removing stop words.
- Feature Extraction: Uses TfidfVectorizer to transform the processed text into TF-IDF features.
- Model Training: Trains a Naive Bayes classifier (MultinomialNB) on the training data.
- Evaluation: Evaluates the model using a confusion matrix and accuracy score.


## Results

After running the script, you will see the accuracy score and confusion matrix printed in the console, indicating the performance of the spam classifier on the dataset.
