# RNN for Text Sentiment Classification

## Project Overview

This project demonstrates how a Recurrent Neural Network (RNN) can be used for binary sentiment classification on text data.

The model learns to classify customer reviews as either:

* Positive (1)
* Negative (0)

A custom dataset of customer feedback sentences was created and used to train the model.

---

## Dataset

Sample reviews used:

* excellent service
* poor service
* very happy with the product
* very disappointed with the product
* delivery was fast
* delivery was late
* highly recommended
* not recommended
* worth buying
* waste of money

Labels:

* 1 → Good
* 0 → Bad

---

## Workflow

### 1. Text Preprocessing

* Tokenization using Keras One-Hot Encoding
* Vocabulary Size = 1000
* Sequence Padding using `pad_sequences()`
* Fixed sequence length for model input

### 2. Embedding Layer

Text tokens are converted into dense vector representations using an Embedding layer.

### 3. RNN Architecture

Model Architecture:

* Embedding Layer
* Masking Layer
* Bidirectional SimpleRNN Layer (10 Units)
* Bidirectional SimpleRNN Layer (15 Units)
* Bidirectional SimpleRNN Layer (20 Units)
* Dense Output Layer (Sigmoid Activation)

### 4. Training

* Loss Function: Binary Crossentropy
* Optimizer: Adam
* Metric: Accuracy
* Batch Size: 1
* Epochs: 2

### 5. Prediction

The trained model can predict sentiment for unseen text reviews.

Example:

Input:

hard to understand topics

Output:

Bad Review

---

## Technologies Used

* Python
* NumPy
* Pandas
* TensorFlow
* Keras
* NLTK

---

## Key Concepts Demonstrated

* Text Encoding
* Sequence Padding
* Word Embeddings
* Recurrent Neural Networks (RNN)
* Bidirectional RNN
* Binary Classification
* Sentiment Analysis

---

## Future Improvements

* Train on larger datasets
* Increase epochs for better accuracy
* Apply dropout regularization
* Compare RNN with LSTM and GRU models
* Deploy using Flask or Streamlit

---

## Learning Outcome

Through this project, I learned:

* How sequential text data is processed
* Working of Simple RNN networks
* Importance of embeddings in NLP
* Bidirectional sequence learning
* Text sentiment classification pipeline

---

## Author

Chaithanya Gollapalli

Aspiring AI/ML Engineer | Python | Machine Learning | Deep Learning | NLP
