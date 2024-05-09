# PyTorch Chatbot

This is a simple chatbot implemented in Python using PyTorch. The chatbot can respond to various intents such as greetings, goodbyes, inquiries about items, payments, delivery, and even tell jokes. It is implemented with a graphical user interface (GUI) using Tkinter.

## How It Works

### Data Preparation

The chatbot is trained on a JSON file containing intents (`intents.json`). Each intent consists of a tag, patterns (user input), and responses. The data is preprocessed by tokenizing the input sentences, stemming the words, and converting them to a bag of words representation.

### Model Training

A neural network model is trained using PyTorch (`train.py`). The model consists of an input layer, multiple hidden layers, and an output layer. The training process involves forward and backward passes, optimizing the weights using Adam optimizer, and minimizing the cross-entropy loss.

### Model Architecture

The neural network architecture is defined in the `model.py` file. It consists of a feedforward neural network with linear layers and ReLU activation functions.

### Chat Logic

The chat logic is implemented in the `chat.py` file. It loads the trained model and uses it to generate responses to user input. The responses are based on the intent with the highest predicted probability, and a threshold is applied to ensure confidence in the response.

### Graphical User Interface (GUI)

The GUI is implemented using Tkinter, a built-in Python library for creating simple desktop applications. It provides a text input field for users to type messages and a text widget to display the conversation history.

## Usage

To run the chatbot, execute the `app.py` file. This will launch the GUI, where you can interact with the chatbot by typing messages in the input field and pressing Enter or clicking the Send button.

## Requirements

- Python 3.x
- PyTorch
- NLTK (Natural Language Toolkit)
- Tkinter (for GUI)

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/ManjotSinghJolly/PyTorch-Chatbot.git
   ```
