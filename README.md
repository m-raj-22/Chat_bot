# Chatbot using Neural Network

## Overview
This project involves developing a chatbot using a neural network model. The chatbot is designed to understand and respond to user inputs based on predefined intents. The model is trained on a dataset of patterns and responses, allowing it to classify user queries into different categories and provide appropriate responses.

## Objectives
- To develop an intelligent chatbot capable of understanding and responding to user inputs.
- To utilize a neural network for intent classification and response generation.
- To implement tokenization, padding, and embedding techniques for text processing.

## Technologies and Tools
- **Programming Language**: Python
- **Libraries**: TensorFlow, Keras, NumPy, Scikit-learn, JSON, Pickle
- **Model Type**: Sequential Neural Network
- **Environment**: Jupyter Notebook or any Python IDE

## Dataset
- **Source**: `intents.json` file containing predefined patterns and responses.
- **Structure**: The file is structured with intents, each having a tag, patterns (input sentences), and responses (output sentences).

## Key Components
### 1. Data Preparation
- Load and parse the `intents.json` file.
- Extract patterns and corresponding tags for training.
- Encode tags into numerical labels using `LabelEncoder`.

### 2. Text Processing
- Tokenize the input sentences using `Tokenizer`.
- Convert tokenized sentences into padded sequences.

### 3. Model Architecture
- **Embedding Layer**: To convert words into dense vectors of fixed size.
- **GlobalAveragePooling1D Layer**: To reduce the dimensionality of the vectors.
- **Dense Layers**: Two fully connected layers with ReLU activation.
- **Output Layer**: Softmax activation to classify intents.

### 4. Training
- Compile the model using `sparse_categorical_crossentropy` loss and `adam` optimizer.
- Train the model with the prepared dataset.

### 5. Model Saving
- Save the trained model using `model.save()`.
- Save the tokenizer and label encoder using `pickle`.

### Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

### License
This project is licensed under the MIT License - see the LICENSE file for details.

### Author
Raj Mehta

© 2024 Raj Mehta
