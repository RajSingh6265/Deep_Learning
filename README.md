![Screenshot 2024-06-22 020526](https://github.com/RajSingh6265/Deep-Learning/assets/157066708/7a589b25-45a8-4b9d-b5a7-6fe8c89e1274)
![Screenshot 2024-06-22 020516](https://github.com/RajSingh6265/Deep-Learning/assets/157066708/91c23567-36c6-46aa-8552-b21bdb679fec)
![Screenshot 2024-06-22 020505](https://github.com/RajSingh6265/Deep-Learning/assets/157066708/6e80217b-e16f-4a17-9ae3-1f59fbef0c1d)
![Screenshot 2024-06-22 020445](https://github.com/RajSingh6265/Deep-Learning/assets/157066708/61486478-37d8-4eb5-83b1-cb556f93d79c)
![Screenshot 2024-06-22 020431](https://github.com/RajSingh6265/Deep-Learning/assets/157066708/3958d637-f774-4cb7-bc47-959649880468)
![Screenshot 2024-06-22 020416](https://github.com/RajSingh6265/Deep-Learning/assets/157066708/cf3c21e1-127e-4a80-8a65-c765a4fc185f)
# Deep-Learning
Next Word Prediction using LSTM

This project demonstrates a neural network model that predicts the next word in a sequence using an LSTM (Long Short-Term Memory) network. The model is built using TensorFlow and Keras and is trained on a dataset containing 5825 unique words. The primary objective is to generate text by predicting the next word based on the context provided by the previous words.

Project Overview
Tokenization
The data is tokenized using Keras' Tokenizer, converting text into sequences of integers. Each unique word is assigned a unique integer.


Dataset Preparation
The input sequences are prepared from the tokenized data. Each sequence is padded to ensure uniform length, which is necessary for training the LSTM model.

Model Architecture

The model comprises:

An Embedding layer with an input dimension of 5826 (vocabulary size + 1) and output dimension of 100.
An LSTM layer with 150 units.
A Dense layer with 5825 units and softmax activation for multi-class classification.

Training
The model is compiled with categorical crossentropy loss and the Adam optimizer. It is trained for 100 epochs.

Prediction
The model predicts the next word in a sequence. It can also generate a sequence of 10 words based on an initial input text.
