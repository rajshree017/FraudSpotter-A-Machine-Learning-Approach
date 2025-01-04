# FraudSpotter-A-Machine-Learning-Approach
This project aims to detect fake reviews in a dataset containing 40,000 reviews across distinct categories like Home and Office, Sports, etc. Each review is labeled as either CG (Computer-Generated) or OR (Original Human-Generated), with accompanying review text and ratings.

The goal is to classify reviews as either fake or authentic based on the text. This project uses advanced text preprocessing techniques and machine learning models to achieve high accuracy in predictions.

# Dataset Overview
Total Reviews: 40,000
20,000 Human-Generated Reviews (OR)
20,000 Computer-Generated Reviews (CG)
# Key Techniques and Tools
Text Preprocessing-
Punctuation removal, stopword elimination, stemming, lemmatization, and digit removal.
Text Vectorization-
CountVectorizer and TF-IDF for transforming text into feature vectors.
Machine Learning Models-
Support Vector Classifier (88% accuracy)
Logistic Regression (86%)
Random Forests & Naive Bayes (84%)
Decision Tree Classifier (73%)
K-Nearest Neighbors (58%)
# Highlights
The Support Vector Classifier (SVC) emerged as the best model, achieving an accuracy of 88%.
Preprocessing and feature engineering played a critical role in performance improvement.
