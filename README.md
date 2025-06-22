# Sentiment-Analysis-of-IMDB-Movie-Reviews-Using-LSTM


**Problem Statement:**
Develop and evaluate an LSTM-based model to perform sentiment analysis on the IMDB Movie Reviews dataset,predicting whether are view is positive or negative.

**Skills Gained**
Text preprocessing techniques for NLP
Sequence modeling with LSTM and Bidirectional LSTM
Model training, validation, and evaluation
Performance visualization (loss & accuracy curves)
Binary classification using deep learning

**Dataset**
Dataset: IMDB Movie Reviews
Source: tf.keras.datasets.imdb
Size:
25,000 training samples
25,000 test samples
Labels: 0 = Negative, 1 = Positive

**Project Workflow**
1. Dataset Loading
Loaded IMDB dataset using tensorflow.keras.datasets.imdb
Inspected structure (integer-encoded sequences and binary labels)

2. Data Exploration
Visualized distribution of review lengths
Analyzed label distribution
Determined vocabulary size and word index mapping

3. Text Preprocessing
Padded sequences to uniform length (maxlen = 200)
Decoded some encoded reviews for interpretability
Cleaned and tokenized custom review inputs

4. Build LSTM Model
Used an Embedding layer to convert tokens into dense vectors
Added LSTM and Bidirectional LSTM layers for sequence modeling
Applied Dropout for regularization

5. Train the Model
Compiled the model with:
Loss: binary_crossentropy
Optimizer: adam
Trained on training set and validated on test set

6. Evaluate the Model
Evaluated performance using:
Accuracy
Precision
Recall
F1 Score
Plotted learning curves (accuracy and loss over epochs)

7. Make Predictions
Predicted sentiment on custom user reviews
Decoded results into Positive or Negative classes


Results
Achieved 86% validation accuracy

