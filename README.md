# English-French Translator using RNN

This project aims to create a language translation application capable of translating English sentences into French. The core of the system is based on a deep neural network, specifically a Recurrent Neural Network (RNN) with Gated Recurrent Units (GRU) for sequence-to-sequence translation.






# Overview
In this project, we utilize a deep neural network to build an end-to-end machine translation pipeline. The steps involved in the process include:

1. Data Loading and Analysis:
  - The English and French sentences are loaded from the provided datasets (small_vocab_en.txt and small_vocab_fr.txt).
  - A brief analysis of the dataset is performed, showcasing a few examples from both languages.
2. Vocabulary Analysis:
  - The vocabulary of both English and French is analyzed to understand the complexity of the dataset.
  - The Counter module is used to count the occurrences of words in each language.
3. Tokenization and Padding:
  - Tokenization is performed on the text data, converting words into numerical sequences.
  - Padding is applied to ensure that all sequences have the same length, essential for feeding data into the neural network.
4. Model Architecture:
  - An RNN model is constructed using GRU nodes for sequence-to-sequence translation.
  - The model includes embedding layers, GRU layers, time-distributed dense layers, dropout layers, and softmax activation.
  - The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss function.
5. Training:
  - The model is trained on the English and French data.
  - Training history, including loss and accuracy metrics, is visualized.
6. Model Saving:
  - The trained model is saved for future use, allowing for efficient re-use without retraining.
7. Inference and Prediction:
  - The model is used for translating English sentences into French.
  - A user interface is provided using Gradio, allowing users to input English text and receive the corresponding French translation.



