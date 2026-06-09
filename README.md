# Sentiment Analysis using Recurrent Neural Network (RNN)

This repository presents a practical Natural Language Processing (NLP) project that implements a **Simple Recurrent Neural Network (RNN)** for binary sentiment classification.

The objective is to demonstrate how recurrent neural networks process sequential text data, learn contextual relationships between words, and classify sentiments as positive or negative using learned word representations.

---

## 🚀 Project Workflow

### 1. Text Data Preparation

* Created a collection of sample text reviews containing positive and negative sentiments.
* Assigned binary sentiment labels:

  * **1 → Positive**
  * **0 → Negative**
* Constructed a supervised learning dataset for sentiment classification.

### 2. Text Preprocessing

* Converted raw text into machine-readable numerical sequences.
* Applied tokenization to build a vocabulary of unique words.
* Mapped each word to a unique integer index.
* Generated padded sequences to ensure uniform input length across all samples.

### 3. Sequence Representation

* Transformed text sentences into fixed-length numerical vectors.
* Applied sequence padding to handle sentences of varying lengths.
* Prepared input data suitable for recurrent neural network training.

---

## 🧠 Model Development

### Embedding Layer

* Converts integer-encoded words into dense vector representations.
* Learns semantic relationships between words during training.
* Produces low-dimensional word embeddings that capture contextual information.

### Simple Recurrent Neural Network (RNN)

* Implemented using TensorFlow/Keras Sequential API.
* Architecture:

  * Embedding Layer
  * SimpleRNN Layer
  * Dense Output Layer (Sigmoid Activation)
* Optimizer: Adam
* Loss Function: Binary Crossentropy

The recurrent layer processes text sequentially, maintaining an internal hidden state that captures information from previously encountered words.

---

## 📊 Results

The RNN successfully learns sentiment-related patterns from the training data and predicts whether unseen text expresses positive or negative sentiment.

Key Observations:

* Captures sequential dependencies in text.
* Learns contextual information through hidden states.
* Demonstrates how word order influences sentiment prediction.
* Provides a foundation for understanding advanced sequence models such as LSTM and GRU networks.

---

## 📈 Hidden State Analysis

One of the primary goals of this project is to visualize how RNNs maintain memory over time.

The notebook includes:

* Inspection of intermediate hidden states.
* Step-by-step processing of word sequences.
* Demonstration of how contextual information accumulates across time steps.
* Understanding of the internal memory mechanism of recurrent networks.

These analyses help explain how RNNs learn representations of sequential text.

---

## 📉 Visualizations Included

The project includes:

* Vocabulary generation and word-index mapping.
* Tokenized sentence representations.
* Padded sequence visualization.
* Embedding representation examples.
* Hidden-state inspection and interpretation.
* Sentiment prediction outputs.

These visualizations provide insight into how textual information flows through an RNN architecture.

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* TensorFlow
* Keras
* Matplotlib
* Scikit-Learn

---

## 📂 Dataset

The project uses a custom sentiment dataset consisting of text reviews labeled as positive or negative.

Target Classes:

```text
0 → Negative Sentiment
1 → Positive Sentiment
```

Input Features:

* Raw text reviews
* Tokenized word sequences
* Padded numerical representations

---

## 🎯 Conclusion

This project demonstrates the fundamental principles of Recurrent Neural Networks for Natural Language Processing tasks.

* The **Embedding Layer** learns meaningful word representations.
* The **Simple RNN** captures sequential dependencies and contextual information.
* Hidden-state analysis provides insight into how recurrent networks maintain memory across time steps.
* The project serves as a strong introduction to sentiment analysis and sequence modeling using deep learning.

The results highlight why recurrent neural networks became an important milestone in NLP and provide a foundation for exploring more advanced architectures such as **LSTM**, **GRU**, and **Transformer-based models**.
