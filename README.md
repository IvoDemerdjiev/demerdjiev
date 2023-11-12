Transformer-based Text Generation

This repository contains a TensorFlow implementation of a text generation model based on the Transformer architecture. The model is trained to generate coherent text based on a given input sequence, and it utilizes multi-head attention mechanisms and feedforward layers.

Problem Statement
The goal of this project is to generate human-like text based on a given prompt or seed text. The Transformer architecture, known for its success in natural language processing tasks, is employed for this text generation task.

Data
The model is trained on the works of William Shakespeare, which is available as a text file. The dataset is preprocessed to create a windowed dataset, which is then used for training and validation.

Model Architecture
The core of the text generation model consists of multi-head attention layers and feedforward layers. The model uses a decoder-only Transformer architecture for simplicity. The decoder includes an embedding layer, positional encoding, dropout, multiple transformer blocks, layer normalization, and a linear layer to project the output to the vocabulary size.

Hyperparameters
The hyperparameters, including batch size, block size, maximum iterations, learning rate, number of embeddings, number of attention heads, number of layers, and dropout rate, are configurable. These values can be adjusted based on the specific requirements of the text generation task.

Training
The model is trained using TensorFlow and compiled with the Adam optimizer and sparse categorical crossentropy loss. The training progress, including loss and validation metrics, is tracked over multiple epochs.
