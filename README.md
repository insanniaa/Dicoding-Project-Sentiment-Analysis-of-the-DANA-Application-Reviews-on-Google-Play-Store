# Sentiment Analysis of the DANA Application Reviews on Google Play Store

This project focuses on performing sentiment analysis on user reviews of the **DANA** application obtained from the Google Play Store.

The goal is to classify user sentiments (positive, neutral, or negative) and evaluate different feature extraction techniques and machine learning algorithms.

## Dataset

The dataset was collected by scraping user reviews of the DANA application from the Google Play Store on **March 9, 2025**. It contains **121,500 rows** and **11 columns**.

### Columns in the Dataset:

- `reviewId`: Unique identifier for the review
- `userName`: Name of the user
- `userImage`: URL to the user's profile image
- `content`: The text content of the review
- `score`: Rating given by the user (1 to 5)
- `thumbsUpCount`: Number of likes the review received
- `reviewCreatedVersion`: App version when the review was written
- `at`: Timestamp of the review
- `replyContent`: Content of the developer's reply
- `repliedAt`: Timestamp of the developer's reply
- `appVersion`: App version being reviewed

## Feature Extraction

Two feature extraction techniques were applied:

- **TF-IDF (Term Frequency-Inverse Document Frequency)**: Converts text data into weighted numerical features.
- **Word2Vec**: Embeds words into vector space using word context.

## Modeling

Different training schemes were implemented by varying:

- **Algorithms**:
  - Support Vector Machine (SVM)
  - Random Forest
  - Logistic Regression

- **Feature Extraction Methods**:
  - TF-IDF
  - Word2Vec

- **Train-Test Splits**:
  - 80:20 split (80% training, 20% testing)
  - 70:30 split (70% training, 30% testing)

The goal was to compare the performance of each combination and identify the most effective approach for sentiment classification.
