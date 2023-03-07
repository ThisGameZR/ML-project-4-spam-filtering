# ML-project-4-spam-filtering

## Spam filtering algorithm:

- Data preprocessing:
  - Lowercasing: Convert all letters to lower case to standardize the text.
  - Number and punctuation removal: Remove any numbers or punctuation marks from the text.
  - Stop word removal: Remove common stop words, such as "a" and "the", that do not contribute much to the classification of the message.
  - Word stemming: Reduce words to their base form to help identify common themes in the text.
  - Word lemmatization: Transform words into their root form to help identify their meaning and improve classification.
  - TF-IDF vectorization: Convert the preprocessed text into a numerical representation that captures the importance of each word or feature in the document relative to the corpus.
- Classifier:
  - Naive Bayes: Use the Multinomial Naive Bayes algorithm to classify the preprocessed text data into spam or ham categories based on the probabilities of the different words or features that are present in the message.

## Performance of model:

- Confusion Matrix

|           | Predicted Ham | Predicted Spam |
|-----------|---------------|----------------|
| Actual Ham   |      1930       |          0            |
| Actual Spam  |       90        |          209          |

  - True Negative (TN): the message is not spam
  - True Positive (TP): the message is spam
  - False Negative (FN): the message is actually spam, but the model predicted it was not
  - False Positive (FP): e.g., the message is not spam, but the model predicted it was
