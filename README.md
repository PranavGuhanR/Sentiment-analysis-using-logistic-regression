[README.md](https://github.com/user-attachments/files/26568171/README.md)
# Twitter Sentiment Analysis with Logistic Regression

This project implements a complete Natural Language Processing (NLP) pipeline to classify the sentiment of tweets as either positive or negative. Unlike using high-level libraries, this implementation builds the core components from scratch using NumPy to provide a deep understanding of the underlying mathematics.

## Key Features
- **Custom Text Preprocessing**: Tokenization, stemming (Porter Stemmer), stopword removal, and regex-based cleaning (removing URLs, hashtags, and handles).
- **Frequency Mapping**: Efficiently mapping word-label pairs to frequencies to build feature vectors.
- **Scratch Implementation**:
    - **Sigmoid Function** for probability mapping.
    - **Gradient Descent** optimization algorithm.
    - **Log Loss** (Cross-Entropy) cost function.
- **Performance Evaluation**: achieving ~99.65% accuracy on the NLTK Twitter dataset.
- **Error Analysis**: Tools to inspect misclassified tweets to understand model limitations.

## Technical Implementation
The model represents each tweet as a 3D vector: `[Bias, Positive_Frequency_Sum, Negative_Frequency_Sum]`. This dimensionality reduction allows for highly efficient training while maintaining high accuracy.

## Dependencies
- Python 3.x
- NumPy
- Pandas
- NLTK
