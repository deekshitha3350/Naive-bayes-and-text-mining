# Naive-bayes-and-text-mining

Blog Sentiment Analysis and Classification

Project Overview

This project focuses on analyzing and classifying blog content based on sentiment and category labels. The dataset contains blog text, which is preprocessed and cleaned before being classified into predefined categories. Additionally, sentiment analysis is performed on each blog post to categorize its overall sentiment (positive, negative, or neutral). A Multinomial Naive Bayes model is used for classification, and TextBlob is used for sentiment analysis. This project also visualizes the sentiment distribution across different categories.

Key tasks involved in this project:

Data Loading and Exploration
Text Preprocessing and Cleaning
Sentiment Analysis
Text Classification Using Multinomial Naive Bayes
Evaluation Using Classification Metrics
Visualization of Sentiment Distribution

Data Description:
The dataset used in this project is blogs.csv, which contains the following columns:

Data: The content of the blog post.
Labels: The target category label of the blog post (e.g., Technology, Health, Politics, etc.).

Data Overview:
Number of Instances: The dataset contains blog posts with their respective categories and content.
Missing Values: Checked for missing data.
Descriptive Statistics: Basic summary statistics of the dataset.

Sentiment Analysis Overview:

Positive Sentiment: Blog posts with a polarity score greater than 0.
Negative Sentiment: Blog posts with a polarity score less than 0.
Neutral Sentiment: Blog posts with a polarity score of 0.

Challenges:

Imbalanced Categories: Some categories may have more samples than others, leading to biased predictions.
Context-Sensitivity in Sentiment Analysis: Sentiment analysis can be challenging as it may not always capture the true sentiment, especially with sarcastic or ambiguous language.
Limited Vocabulary: The vocabulary used in the training set may limit the model’s ability to understand more complex or domain-specific terms.

Insights from Sentiment Analysis:

Positive Sentiments: Categories with predominantly positive sentiments may reflect uplifting or optimistic topics.
Neutral Sentiments: Neutral sentiments may suggest informative or balanced content.
Negative Sentiments: Categories with negative sentiments may highlight controversial or critical themes in blog posts.

Installation:

To run this project, you need to install the following dependencies:

nltk: For text preprocessing and tokenization.
pandas: For data manipulation.
numpy: For numerical operations.
matplotlib and seaborn: For data visualization.
sklearn: For machine learning models and evaluation metrics.
textblob: For sentiment analysis.

How to Run:

Clone this repository to your local machine.
Place the blogs.csv file in the root directory of the project.
Run the sentiment_analysis_and_classification.py script to preprocess the data, train the model, and visualize the results.

Data Loading and Preprocessing:

Load the CSV file using pandas.
Clean the text data by removing non-alphanumeric characters and stopwords.

Feature Extraction:
Use TF-IDF Vectorization to convert text data into numerical features for classification.

Model Training and Evaluation:

Train the Multinomial Naive Bayes classifier on the processed data.
Evaluate the model performance using accuracy and classification metrics (Precision, Recall, F1-Score).

Sentiment Analysis:

Perform sentiment analysis on each blog post using TextBlob.
Visualize the sentiment distribution across different categories.

Results:

Final Accuracy: Evaluates the accuracy of the Multinomial Naive Bayes model.
Classification Report: Provides detailed precision, recall, and F1-score for each class.
Confusion Matrix: Displays the confusion matrix to visualize model performance.
