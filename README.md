# Sentiment Analysis: Naive Bayes

## Project Overview

This repository contains the code for a sentiment analysis model built using the Naive Bayes classifier algorithm. The model is designed to classify text data into sentiment categories i.e. positive or negative.

## Project Description

Sentiment analysis is a crucial task in natural language processing (NLP), aiming to understand and classify the emotional tone expressed in text. This project focuses on building a sentiment analysis model using the Naive Bayes algorithm, a probabilistic machine learning approach.

### Motivation:

Sentiment analysis has numerous real-world applications, including:

  **Social Media Monitoring:** Tracking public opinion and brand sentiment on social media platforms.
  **Customer Feedback Analysis:** Understanding customer satisfaction and identifying areas for improvement in products or services.
  **Market Research:** Analyzing customer reviews and market trends to inform business decisions.
  **Political Analysis:** Gauging public opinion on political issues and candidates.

### Target Audience:

This project is intended for data scientists, machine learning enthusiasts, and students interested in exploring the fundamentals of natural language processing and sentiment analysis.

## Key Highlights:

* **Data Preprocessing:** Handling of tweets through tokenization, stopword removal, and vectorization
* **Modeling:** Training Naive Bayes Classifier from scratch and using it to predict sentiment.
* **Evaluation:** Model performance is evaluated using *accuracy* metric

## Project Setup
### Dataset

The dataset used in this project contains textual data (e.g., product reviews, tweets, or movie reviews) that are labeled as positive or negative. You can use any publicly available dataset for sentiment analysis (e.g., the IMDB reviews dataset or Twitter sentiment dataset).

### Steps in the Project

* Data Preprocessing:
    - Train-Test Splitting: Dividing the dataset into training and testing parts
    - Visualization: Implementing visual graphs to understand the input data
    - Text Cleaning: Removing special characters, numbers, and stopwords.
    - Tokenization: Breaking text into individual words.
    - Frequency Dictionary: Counting the number of times a word appeared with its respective sentiment (1 for positive and 0 for negative)

* Model Training:
    - Naive Bayes Classifier is trained on the processed text data to predict sentiment labels.

* Model Evaluation:
    - The model's performance is evaluated on a held-out test set using the accuracy metric.

### Files in the Repository
   - sentiment-analysis-nb.ipynb: The jupyter notebook containing the main project code
   - utils.py: Contains the helper functions that are utilized in the main notebook
   - w2_unittest.py: Contains manually written test cases to check function correctness in the main script
   - freqs_dict.pkl: Sample file showing how frequency dictionary must look like:
       - **Key:** A Tuple (word, sentiment (1 or 0))
       - **Value:** Frequency of that tuple
   - loglikelihood_test.pkl: Sample file showing log likelihood of each word
   - README.md: This file.

## Model Performance
Once the model is trained and evaluated, the results will be displayed, showing how well the model performs on the test set. Error Analysis is also performed to observe which tweets from the test set were incorrectly classified. Additionally, users will be allowed to type in their own tweets and let the trained model classify it (at the end of the main notebook).

### Sample Output
- Naive Bayes accuracy = 99.55 %

The accuracy metric helps you understand how well the model is classifying the sentiment of the text.

### Example
**Input Text:** "This is a ridiculously bright movie. The plot was terrible and I was sad until the ending!"

**Predicted Sentiment:** Negative 

## Acknowledgements

* Dataset sources:
  * [Twitter](https://www.x.com)   
  * [Coursera](https://www.coursera.org/)
    
* Libraries used:
  * NumPy for vectorized calculations.
  * Pandas for data handling.
  * NTLK for accessing tweets dataset.
