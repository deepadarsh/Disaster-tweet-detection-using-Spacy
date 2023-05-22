# Disaster Tweets Classification

This project aims to classify tweets as either disaster-related or not using machine learning algorithms. The goal is to build a model that can accurately identify tweets that are relevant to disasters, which can be useful for various applications such as disaster response and management.

## Dataset

The dataset used in this project is taken from the "Disaster Tweets" dataset. It contains a collection of tweets labeled as disaster-related or not. The dataset includes the following columns:
- `text`: The original text content of the tweet
- `target`: The binary label indicating whether the tweet is disaster-related (1) or not (0)

## Approach

The classification task is performed using several machine learning algorithms and techniques. The following steps are performed:

1. Data Preprocessing:
   - The text data is cleaned by removing URLs, special characters, and punctuation.
   - Stopwords are removed to eliminate common words that do not contribute much to the classification task.
   - The text is tokenized and lemmatized to convert words into their base form.

2. Feature Extraction:
   - CountVectorizer is used to convert the preprocessed text data into numerical feature vectors.

3. Model Training:
   - Logistic Regression:
     - A logistic regression model is trained on the training data.
     - The best hyperparameters are determined using GridSearchCV.
     - The accuracy of the model is evaluated using the ROC AUC score.

   - XGBoost:
     - The training and test data are converted to DMatrix format.
     - XGBoost parameters are defined, such as maximum depth and learning rate.
     - The XGBoost classifier is trained on the training data.
     - The performance of the model is evaluated using the ROC AUC score.

## Results

The performance of the models on the test data is as follows:
- Logistic Regression: ROC AUC score of 0.80
- XGBoost: ROC AUC score of 0.76



## Conclusion

In this project, we developed models to classify disaster-related tweets using machine learning algorithms. The logistic regression and XGBoost models achieved 0.80. These models can be further refined and used to analyze and classify tweets in real-time to assist in disaster response efforts.

Feel free to explore the code, experiment with different algorithms, and contribute to the project!



