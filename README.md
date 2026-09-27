# IMDb Sentiment Analysis using RNN

## Project Overview

This project develops a sentiment analysis system using a Recurrent Neural Network (RNN) to classify IMDb movie reviews as **Positive** or **Negative**.

The model learns sequential relationships between words in movie reviews and predicts the sentiment of the review.

## Objective

The main objective of this project is to build an RNN-based text classification model that can automatically identify the sentiment of IMDb movie reviews.

- Positive → 1
- Negative → 0

## Dataset

The project uses the **IMDb Movie Reviews dataset** available through TensorFlow/Keras.

- Training samples: 25,000
- Testing samples: 25,000
- Vocabulary size: 10,000 words
- Maximum review length: 200 words

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Model Architecture

The RNN model consists of:

1. **Embedding Layer** – Converts word indexes into dense vector representations.
2. **SimpleRNN Layer** – Learns sequential relationships between words.
3. **Dense Layer** – Performs binary sentiment classification using sigmoid activation.



## Data Preprocessing

The IMDb reviews are already represented as numerical sequences.

Padding is applied to make all reviews have a fixed length of **200**. This allows the RNN to receive inputs of the same size.

## Model Training

The model was trained for 5 epochs using the training dataset with a validation split of 20%.

The final training accuracy reached approximately **99.07%**, while the validation accuracy was approximately **79.16%**.

The difference between training and validation performance indicates possible overfitting.

## Model Evaluation

The trained model was evaluated using standard classification metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

These metrics help measure how effectively the model classifies positive and negative movie reviews.

## Prediction

After training, the model generated predictions for the IMDb test dataset.

A probability threshold of **0.5** was used:

- Probability ≥ 0.5 → Positive
- Probability < 0.5 → Negative

## New Review Testing

The model was also tested with a new movie review to demonstrate how the trained RNN can classify unseen text as positive or negative.

## Results

The model successfully learned sentiment patterns from IMDb movie reviews.

The training and validation graphs were used to analyze model learning, while classification metrics and the confusion matrix were used to evaluate the model's performance.


## Conclusion

An RNN-based sentiment analysis system was successfully developed using IMDb movie reviews. The model learned sequential patterns in the review text and classified reviews into positive and negative sentiments.

The model performance was analyzed using accuracy and loss graphs and evaluated using accuracy, precision, recall, F1-score, confusion matrix, and classification report.

This project demonstrates how Recurrent Neural Networks can be used for text classification and sentiment analysis.
